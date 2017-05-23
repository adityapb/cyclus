FROM cyclus/cyclus-deps

COPY . /cyclus
WORKDIR /cyclus
ENV PATH="/root/.local/bin:${PATH}"
RUN python install.py -j2 --build-type=Release --core-version 999999.999999
RUN cp /root/.local/bin/cyclus /usr/bin/cyclus_exec
RUN mkdir /usr/lib/cyclus
RUN cp /root/.local/lib/cyclus/* /usr/lib/cyclus
RUN cp /root/.local/lib/libcyclus.so /usr/lib
RUN cp /usr/lib/liblapack.so.3 /usr/bin/liblapack.so.3


FROM cyclus/cyclus-deps

COPY . /cyclus
WORKDIR /cyclus
ENV PATH="/root/.local/bin:${PATH}"
RUN python install.py -j2 --build-type=Release --core-version 999999.999999
RUN ln -s /root/.local/bin/cyclus /usr/bin/cyclus_exec
RUN ln -s /root/.local/lib/cyclus/* /usr/lib/cyclus
RUN ln -s /root/.local/lib/libcyclus.so /usr/lib
RUN ln -s /usr/lib/* /usr/bin


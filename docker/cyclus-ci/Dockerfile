FROM cyclus/cyclus-deps

COPY . /cyclus
WORKDIR /cyclus
ENV PATH="/usr/bin:/usr/lib:${PATH}"
RUN python install.py -j2 --build-type=Release --core-version 999999.999999
RUN cp /root/.local/bin/cyclus /usr/bin/cyclus_exec
RUN mv /root/.local/lib/cyclus/ /usr/lib/cyclus
RUN cp /root/.local/lib/libcyclus.so /usr/lib


FROM cyclus/cyclus-deps

COPY . /cyclus
WORKDIR /cyclus
ENV PATH="/usr/bin:/usr/lib:${PATH}"
RUN mkdir build
RUN cd build
RUN cmake .. -DCMAKE_INSTALL_PREFIX=/usr/
RUN make
RUN make install


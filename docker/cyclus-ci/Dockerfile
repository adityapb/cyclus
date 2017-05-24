FROM cyclus/cyclus-deps

COPY . /cyclus
WORKDIR /cyclus
ENV PATH="/usr/bin:/usr/lib:${PATH}"
RUN mkdir cyclus/build
RUN cd cyclus/build && cmake .. -DCMAKE_INSTALL_PREFIX=/usr/ && make && make install


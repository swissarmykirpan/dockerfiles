FROM minimum2scp/ruby-full:latest
MAINTAINER YAMADA Tsuyoshi <tyamada@minimum2scp.org>

COPY build /build
RUN run-parts --report --exit-on-error /build/scripts && rm -rf /build
EXPOSE 22 80 9001

ENTRYPOINT ["/opt/init-wrapper/sbin/entrypoint.sh"]
CMD ["/sbin/init"]


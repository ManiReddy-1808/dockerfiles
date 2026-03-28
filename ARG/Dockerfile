# ARG can be the 1st instruction in a special case to supply the version to base image.
# ARG is for FROM instruction, it should be before the FROM instruction. It is only available during build time and not available during runtime.

ARG version
FROM almalinux:${version:-8}
# If not provided version, it will take 8 as default version.

ARG COURSE="Docker" \
    TRAINER="Sivakumar" \
    DURATION="10HRS" \
    AUTHOR="joindevops"
RUN echo "Trainer is: ${TRAINER}, version is: ${version}"
CMD ["sleep", "200"]

# EX: docker build -t arg:1.0.0 --build-arg version=9 .
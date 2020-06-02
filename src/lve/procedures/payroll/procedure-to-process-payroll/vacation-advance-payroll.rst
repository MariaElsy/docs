.. _ERPyA: http://erpya.com
.. |Nómina Anticipo de Vacaciones| image:: resources/anticipovacaciones.png
.. |Incidencias Nómina Anticipo de Vacaciones| image:: resources/anticipovacaciones.png
.. |Recibo de Pago Nómina Anticipo Vacaciones| image:: resources/reciboanticipovacaciones.png
.. |Detalle de Pago Nómina Anticipo Vacaciones| image:: resources/detalleanticipovacaciones.png
.. |Resumen de Pago Nómina Anticipo Vacaciones| image:: resources/resumenanticipovacaciones.png
.. |Retenciones Nómina Anticipo Vacaciones| image:: resources/retencionesanticipovacaciones.png
.. |Aportes Nómina Anticipo Vacaciones| image:: resources/aportesaanticipovacaciones.png

.. _documento/nomina-anticipo-vacaciones:

==================================
**Nómina Anticipo de Vacaciones**
==================================

Para procesar una “**Nómina de Anticipo de Vacaciones**” debemos realizar el proceso de nómina estándar mencionado en el documento :ref:`documento/procedimiento-para-procesar-nómina` elaborado por `ERPyA`_. En esta ventana se registran los datos principales que ADempiere requiere para crear una nómina de anticipo de vacaciones, el comportamiento de esta nómina destaca que solo existirá la asignación de días de disfrute de vacaciones, la asignación de bono vacacional y cualquier otra asignación estarán  representadas solamente en la nómina de vacaciones, cada uno de los campos detallados a continuación son relevantes para obtener un registro exitoso:


#. Estatus del Documento:

    #. Seleccione “**Nómina  Vacaciones**” en el campo “**Tipo de Documento**”

        El tipo de documento le permitirá definir la acción del documento que esté registrando en ADempiere.

    #. Selecciones “**Nómina Anticipo de Vacaciones**” en el campo “**Nómina**”

	   La nómina de anticipo de vacaciones define el comportamiento de la nómina, para este caso por ser una nómina especial cuenta con las siguientes características:

            #. Regla de Pago: Débito Directo
            #. Contrato de Nómina: Contrato Mensual
            #. Cargo: Vacaciones por Pagar

    #. Seleccione la fecha en la que esté ejecutando la nómina en el campo **Fecha Contable**


    #. Seleccione el “**Socio de Negocio Empleado**” a quién se le procesa la nómina de anticipo de vacaciones en el campo **Socio de Negocio**


      |Nómina Anticipo de Vacaciones|

      Imagen 1. Nómina Anticipo de Vacaciones

    .. warning::

        Está nómina  por ser una nómina especial no debe registrarse con período


#. Incidencias:

      Para esta nómina son obligatorias las incidencias, es decir, que antes de procesar la nómina de anticipo de vacaciones debe registrar al empleado las siguientes incidencias


      +-------------------------------------------------------+----------------------+----------------+
      |           **INCIDENCIA**                              |     **CÓDIGO**       |    **TIPO**    |
      +=======================================================+======================+================+
      | Fecha de Inicio de Anticipo de Vacaciones             |     ("IN_FIAV")      |       Fecha    |
      +-------------------------------------------------------+----------------------+----------------+
      | Días de Anticipo de Vacaciones                        |      ("IN_DAV")      |     Cantidad   |
      +-------------------------------------------------------+----------------------+----------------+

    |Incidencias Nómina Anticipo de Vacaciones|

    Imagen 2. Incidencia Nómina Anticipo de Vacaciones

      Para conocer cómo registrar una incidencia puede utilizar el siguiente enlace :ref:`documento/novedades-de-nómina:`

#. Resultados:

    - **Reportes**

    Para visualizar los reportes de nóminas  puede seguir los pasos que se encuentran en el documento :ref:`documento/reporte-de-nómina:` con los datos adicionales que se indican a continuación para cada reporte


        - “**Recibo de Pago**”

         	- **Nómina**: Nómina Anticipo de Vacaciones

         	- **Proceso de Nómina**: Ubique el número de documento del proceso de nómina que está ejecutando.

         	- **Configuración de Reporte de Nómina**: Anticipo de Vacaciones

        |Recibo de Pago Nómina Anticipo Vacaciones|

        Imagen 3. Recibo de Pago Nómina Anticipo de Vacaciones


        - “**Detalle de Pago**”

            - **Nómina**: Nómina Anticipo de  Vacaciones

            - **Proceso de Nómina**: Ubique el número de documento del proceso de nómina que está ejecutando.

            - **Configuración de Reporte de Nómina**: Anticipo de Vacaciones

            - **Plantilla de Reporte de Nómina**: Detalle de Pago

        |Detalle de Pago Nómina Anticipo Vacaciones|

        Imagen 4. Detalle de Pago Nómina Anticipo de Vacaciones


        - “**Resumen de Pago**”

            - **Nómina**: Nómina Anticipo de Vacaciones

            - **Proceso de Nómina**: Ubique el número de documento del proceso de nómina que está ejecutando.

            - **Configuración de Reporte de Nómina**: Anticipo de Vacaciones

            - **Plantilla de Reporte de Nómina**: Resumen de Pago


        |Resumen de Pago Nómina Anticipo Vacaciones|

        Imagen 5. Resumen de Pago Nómina Anticipo Vacaciones

        - “**Retenciones**”

            - **Nómina**: Nómina Anticipo de Vacaciones

            - **Proceso de Nómina**: Ubique el número de documento del proceso de nómina que está ejecutando.

            - **Configuración de Reporte de Nómina**: Retenciones Parafiscales

        |Retenciones Nómina Anticipo Vacaciones|

        Imagen 6. Retenciones Nómina Anticipo Vacaciones

        - “**Aportes**”

            - **Nómina**: Nómina Anticipo de Vacaciones

            - **Proceso de Nómina**: Ubique el número de documento del proceso de nómina que está ejecutando.

            - **Configuración de Reporte de Nómina**: Aportes Parafiscales

        |Aportes Nómina Anticipo Vacaciones|

        Imagen 7. Aportes Nómina Anticipo de Vacaciones

        .. note::

            Cabe destacar que los reportes de Aportes y Retenciones se deben pasar al Departamento de Contabilidad

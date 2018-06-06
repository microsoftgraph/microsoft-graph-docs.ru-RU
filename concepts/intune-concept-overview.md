# <a name="intune-devices-and-apps-api-overview"></a>Обзор API устройств и приложений Intune

Microsoft Intune помогает предприятиям управлять устройствами и приложениями в организации. С помощью API Intune в Microsoft Graph вы можете управлять устройствами и приложениями, а также настраивать Intune, используя привычные средства. 

Если вы независимый поставщик программного обеспечения, вы также можете использовать API Intune для управления клиентами.

## <a name="why-integrate-with-intune"></a>Преимущества интеграции с Intune

Вы также можете использовать API Intune в Microsoft Graph для доступа к сведениям об устройствах и приложениях из Intune, управления приложениями и автоматизации Intune.

### <a name="manage-devices"></a>Управление устройствами

С помощью API Intune вы можете:

- Определять и применять политики [соответствия устройств различным требованиям](../api-reference/v1.0/resources/intune_deviceconfig_devicecomplianceactionitem.md), таким как сложность и длина пароля, шифрование, уровни защиты от угроз.  (То, поддерживается ли политика, зависит от используемой операционной системы и ее версии.)
- [Защищать данные компании](../api-reference/v1.0/resources/intune_mam_windowsinformationprotectionpolicy.md) независимо от платформы устройства (Windows, Android, Mac или iOS).
- Создавать и развертывать политики [конфигурации устройств](../api-reference/v1.0/resources/intune_deviceconfig_deviceconfiguration.md), включая платформы и версии операционной системы, членство в доменах и управление параметрами конфигурации.
- Создавать и развертывать политики [контроля доступа](../api-reference/v1.0/resources/intune_onboarding_onpremisesconditionalaccesssettings.md) для устройств, включая ограниченную загрузку, доступ к сетевым аксессуарам и передачу данных.
- Выполнять [удаленные действия](../api-reference/v1.0/resources/intune_devices_manageddevice.md), например поиск устройства, изменение пароля и стирание данных устройства.

### <a name="manage-apps"></a>Управление приложениями 

С помощью API Intune вы можете выполнять указанные ниже задачи по управлению приложениями.

- Развертывание [приложений на устройствах](../api-reference/v1.0/resources/intune_apps_mobileapp.md) и запрет развертывания приложений.
- Управление доступом к [электронным книгам](../api-reference/v1.0/resources/intune_books_ebookinstallsummary.md) и соответствующим службам.
- Определение и развертывание параметров конфигурации и защиты приложений, а также политик их использования.

### <a name="automate-intune"></a>Автоматизация Intune

Автоматизируйте Intune, используя API Intune:

- для определения и назначения правил доступа [на основе ролей](../api-reference/v1.0/resources/intune_rbac_conceptual.md);
- аудита и создания отчетов о соответствии требованиям, использовании и доступе;
- управления [затратами на телекоммуникации](../api-reference/v1.0/resources/intune_tem_conceptual.md).


## <a name="next-steps"></a>Дальнейшие действия

- [Доступ к интерфейсам API Intune в Microsoft Graph с использованием Azure AD](https://docs.microsoft.com/intune/intune-graph-apis).
- Узнайте, как выполнять распространенные задачи, с помощью [примеров PowerShell для Intune](https://github.com/microsoftgraph/powershell-intune-samples).
- Узнайте, как [использовать REST API Intune](https://developer.microsoft.com/ru-RU/graph/docs/api-reference/v1.0/resources/intune_graph_overview).
- Сведения о новых возможностях API Intune см. в [журнале изменений](changelog.md).
- Изучите [примеры](https://developer.microsoft.com/ru-RU/graph/graph/examples) с новыми идеями о том, как использовать Microsoft Graph.

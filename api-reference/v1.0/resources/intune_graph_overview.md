# <a name="working-with-intune-in-microsoft-graph"></a>Работа с Intune в Microsoft Graph  

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/ru-RU/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.

API Microsoft Graph для Intune обеспечивает программный доступ к сведениям Intune для клиента. API выполняет операции Intune, аналогичные доступным с помощью **портала Azure**.  

В сценариях управления мобильными устройствами (MDM) API Graph для Intune поддерживает автономные развертывания. [Гибридные развертывания](https://docs.microsoft.com/ru-RU/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) Intune не поддерживаются. 

## <a name="using-the-intune-graph-api"></a>Использование API Graph для Intune

Intune предоставляет данные интерфейсу API Microsoft Graph аналогично другим облачным службам, предоставляя обширные сведения об объектах и обеспечивая навигацию по связям.  С помощью API Microsoft Graph вы можете объединить данные из других служб и Intune, чтобы создать используемых в разных службах полнофункциональные приложения для ИТ-специалистов и пользователей.     

Ниже приведен пример того, как определить, установлено ли приложение на устройстве пользователя. 

1. Из Azure Active Directory извлеките список устройств, зарегистрированных для пользователя: 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. Затем просмотрите список приложений для вашего клиента: 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. На основе идентификатора, указанного в приложении, определите состояние установки для приложения (и, следовательно, пользователя):

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-permission-scopes"></a>Использование областей разрешений

API Microsoft Graph управляет доступом к ресурсам, используя области разрешений. Разработчикам необходимо указать области разрешений, необходимые для доступа к ресурсам Intune. Как правило, требуемые области разрешений указываются на портале Azure Active Directory. Дополнительные сведения см. в статье об [областях разрешений в Microsoft Graph](https://developer.microsoft.com/ru-RU/graph/docs/authorization/permission_scopes) и [областях разрешений в Intune](https://developer.microsoft.com/ru-RU/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).


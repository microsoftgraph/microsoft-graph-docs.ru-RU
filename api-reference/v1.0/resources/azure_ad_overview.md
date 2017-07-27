# <a name="working-with-azure-active-directory-resources-in-microsoft-graph"></a>Работа с ресурсами Azure Active Directory в Microsoft Graph

Microsoft Graph предоставляет доступ к ресурсам [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/active-directory-whatis) для управления ролями администратора (каталога), приглашения внешних пользователей в организацию, и, если вы являетесь [поставщиком облачных решений](https://partner.microsoft.com/cloud-solution-provider), управления данными клиентов.  Microsoft Graph также предоставляет методы, которые могут использоваться приложениями, например для поиска информации о транзитивных группах и ролях пользователей. 

> **Примечание**. Некоторые ресурсы Azure AD описаны в других разделах справочника по API. Дополнительную информацию см. в статьях [Пользователи](users.md) и [Группы](group.md).


## <a name="authorization"></a>Авторизация
 
Для вызова API Microsoft Graph для ресурсов Azure AD приложению необходимы соответствующие разрешения. Для многих API, предоставляемых для ресурсов Azure AD, требуется одно из [разрешений _Directory_](../../../concepts/permissions_reference.md#directory-permissions). Разрешения Directory дают широкие права и всегда предоставляются администратором. 

Чтобы приложение могло вызывать API AD Azure от имени пользователя (делегированные разрешения), этому пользователю должна быть назначена соответствующая [роль администратора](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles).

Дополнительные сведения о разрешениях, в том числе делегированных и для приложений, см. в [справочнике по разрешениям](../../../concepts/permissions_reference.md). 

## <a name="common-use-cases"></a>Основные варианты использования 

В следующей таблице перечислены основные варианты использования ресурсов Azure AD.

| **Варианты использования**        | **Ресурсы REST** | **См. также** |
|:---------------|:--------|:----------|
| **Объект и методы каталога** | | |
| `directoryObject` — это базовый класс, от которого наследуются многие ресурсы каталога, такие как пользователи и группы. Microsoft Graph предоставляет несколько методов, которые можно использовать для поиска сведений о пользователях, группах и других объектах каталога. Например, вы можете проверить транзитивное членство в списке групп, вернуть все группы и роли, транзитивным членом которых является объект каталога, или получить все ресурсы указанного типа (такие как пользователь или группа) из списка идентификаторов ролевых ресурсов. | [directoryObject](../resources/directoryobject.md) | Недоступно |
| **Управление ролями каталога (администратора)** | | |
| Активируйте роли каталога в клиенте Azure AD и управляйте членством пользователей в ролях каталога. Роли каталога также известны как роли администратора. | [directoryRole](../resources/directoryrole.md) <br/>[directoryRoleTemplate](../resources/directoryroletemplate.md) | [Назначение ролей администратора в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles) |
| **Управление устройствами** | | |
| Управляйте устройствами, зарегистрированными в организации. Устройства (ноутбуки, настольные компьютеры, планшеты и мобильные телефоны) регистрируются на пользователей. Устройства обычно создаются в облаке с помощью службы регистрации устройств или Microsoft Intune. Они используются политиками условного доступа для многофакторной аутентификации. | [device](../resources/device.md) | [Знакомство с регистрацией устройств в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-device-registration-overview).<br/><br/>[Что такое InTune?](https://docs.microsoft.com/intune-classic/understand-explore/introduction-to-microsoft-intune)<br/><br/>[Регистрация устройств для управления в Intune](https://docs.microsoft.com/intune-classic/deploy-use/enroll-devices-in-microsoft-intune) |
| **Управление клиентами партнеров** | | |
| Получайте сведения об отношениях партнерства с клиентами.<br/><br/>**Примечание.** Это относится только к клиентам партнеров. Клиенты партнеров — это клиенты Azure AD, которые принадлежат партнерам корпорации Майкрософт, являющимся [поставщиками облачных решений Майкрософт](https://partnercenter.microsoft.com/partner/programs), участниками программы синдикации Office 365 или участниками партнерской программы Microsoft Advisor. | [contract](../resources/contract.md) | [Вызов Microsoft Graph из приложения Cloud Solution Provider](../../../concepts/auth_cloudsolutionprovider.md) |
| Управляйте доменами, связанными с клиентом. С его помощью регистраторы могут автоматизировать связь домена для таких служб, как Office 365. | [domain](../resources/domain.md) | [Добавление имени личного домена в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-domains-add-azure-portal) |
| **Управление клиентами** | | |
| Получайте информацию об организации, например адрес, контакты для уведомлений и связи по техническим вопросам, планы обслуживания, на которые она подписана, и связанные с ней домены. | [organization](../resources/organization.md) | Недоступно |
| Получайте информацию о службах, на которые подписана компания. | [subscribedSku](../resources/subscribedsku.md) | Недоступно |
| Приглашайте внешних пользователей в организацию. | [invitation](../resources/invitation.md) | [Что такое служба совместной работы Azure AD B2B?](https://docs.microsoft.com/azure/active-directory/active-directory-b2b-what-is-azure-ad-b2b) |



## <a name="next-steps"></a>Дальнейшие действия
Ресурсы и API каталога открывают новые способы взаимодействия с пользователями и контроля их работы с помощью Microsoft Graph. Чтобы узнать больше: 

- Изучите подробнее методы и свойства ресурсов, наиболее полезных для вашего сценария.
- Опробуйте API в [песочнице Explorer](https://developer.microsoft.com/graph/graph-explorer).

Нужны идеи? Посмотрите, [как наши партнеры используют Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).



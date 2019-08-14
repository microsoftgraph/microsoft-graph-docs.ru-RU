---
title: Новые возможности Microsoft Graph
description: Текущие новые возможности в Microsoft Graph
author: angelgolfer-ms
localization_priority: Priority
ms.openlocfilehash: 2e2c608cf05f22ccf9e296520624d7c96fe2b4ce
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367108"
---
# <a name="whats-new-in-microsoft-graph"></a>Новые возможности Microsoft Graph

Знаете ли вы, что некоторые новые возможности Microsoft Graph реализуются на основе распространенных запросов сообщества разработчиков? 

Команда разработчиков Microsoft Graph регулярно оценивает потребности клиентов и выпускает новые функции в следующем порядке.

1. Дебютный выпуск в **_предварительной_** версии. Все соответствующие обновления REST API доступны в конечной точке бета-версии (`https://graph.microsoft.com/beta`).  

2. Повышение до **_общедоступного_ состояния (GA)**, если целесообразность этого подтверждена достаточным количеством отзывов. Все соответствующие обновления REST API добавляются в конечную точку версии 1.0 (`https://graph.microsoft.com/v1.0`). 

Ниже представлен обзор новых возможностей Microsoft Graph и способов [поделиться своими идеями](#want-to-stay-in-the-loop). Подробные сведения об обновлениях API см. в разделах журнала изменений API за [июль](changelog.md#august-2019) и [август](changelog.md#july-2019). 


## <a name="july-2019-new-and-generally-available"></a>Июль 2019 г.: новые и общедоступные возможности 

### <a name="example-code-snippets"></a>Примеры фрагментов кода
Теперь имеются фрагменты кода Objective-C для всех статей по API в справочных материалах для версии 1.0 и бета-версии. См. пример Objective-C для [получения события](/graph/api/event-get?view=graph-rest-1.0&tabs=objective-c#example).

### <a name="group"></a>Группа
- Используйте функцию [validateProperties](/graph/api/group-validateproperties?view=graph-rest-1.0), чтобы отображаемое имя или почтовый псевдоним существующей группы Office 365 соответствовали политикам именования.
- Кроме того, перед созданием группы вы можете использовать функцию [validateProperties](/graph/api/directoryobject-validateproperties?view=graph-rest-1.0) для объекта [directoryObject](/graph/api/resources/directoryobject?view=graph-rest-1.0), чтобы сначала проверить имена.

### <a name="identity-and-access"></a>Удостоверение и доступ
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#organization-permissions) _Organization.Read.All_ и _Organization.ReadWrite.All_ для доступа к [организации](/graph/api/resources/organization?view=graph-rest-1.0) и соответствующим ресурсам, например [SKU, на которые оформлена подписка](/graph/api/resources/subscribedsku?view=graph-rest-1.0).
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#role-management-permissions) _RoleManagement.Read.Directory_ и _RoleManagement.ReadWrite.Directory_ для управления доступом на основе ролей (RBAC) в каталоге компании:

  - Используйте разрешение на чтение и запись, чтобы сначала [активировать](/graph/api/directoryrole-post-directoryroles?view=graph-rest-1.0) роль каталога. 
  - Если роль активирована, вы можете использовать разрешение на чтение для [чтения ролей каталога](/graph/api/directoryrole-list?view=graph-rest-1.0), [перечисления участников ролей](/graph/api/directoryrole-list-members?view=graph-rest-1.0) и [перечисления шаблонов для ролей каталогов](/graph/api/directoryroletemplate-list?view=graph-rest-1.0). 
  - Вы также можете использовать разрешение на чтение и запись для [добавления](/graph/api/directoryrole-post-members?view=graph-rest-1.0) и [удаления](/graph/api/directoryrole-delete-member?view=graph-rest-1.0) участников ролей.


## <a name="july-2019-new-in-preview"></a>Июль 2019 г.: новые возможности предварительной версии

> [!IMPORTANT]
> Функции в состоянии _предварительной версии_, в том числе API и инструменты, могут меняться без предварительного уведомления, а некоторые из них, возможно, никогда не будут повышены до общедоступной версии. Не используйте их в приложениях для рабочей среды.

### <a name="calendar"></a>Календарь 
Используйте новый [API мест](/graph/api/resources/place?view=graph-rest-beta), чтобы применять различные типы расположений, например [помещения](/graph/api/resources/room?view=graph-rest-beta) и [список помещений](/graph/api/resources/roomlist?view=graph-rest-beta), настроенные администраторами Exchange Online.

### <a name="devices-and-apps"></a>Устройства и приложения
Обновления Intune за [июль](changelog.md#july-2019)

### <a name="files"></a>Файлы 
Применяйте дату и время окончания срока действия или пароль при [создании ссылки для общего доступа](/graph/api/driveitem-createlink?view=graph-rest-beta) к файлу, папке или другому объекту [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta).

### <a name="identity-and-access"></a>Удостоверение и доступ
- Используйте [новое разрешение приложений](/graph/permissions-reference?#accessreviews-permissions) _AccessReview.ReadWrite.Membership_ для операций CRUD при [проверках доступа](/graph/api/resources/accessreviews-root?view=graph-rest-beta). 
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#administrative-units-permissions) _AdministrativeUnit.Read.All_ и _AdministrativeUnit.ReadWrite.All_ для чтения и записи (включая создание, обновление и удаление участников, а также управление ими) ресурсов [административных единиц](/graph/api/resources/administrativeunit?view=graph-rest-beta) соответственно.
- Используйте [новые разрешения приложений и делегированные разрешения](permissions-reference.md#organization-permissions) _Organization.Read.All_ и _Organization.ReadWrite.All_ для доступа к [организации](/graph/api/resources/organization?view=graph-rest-beta) и соответствующим ресурсам, например [SKU, на которые оформлена подписка](/graph/api/resources/subscribedsku?view=graph-rest-beta).
- Используйте новую функцию [обнаружения](/graph/api/directorydefinition-discover?view=graph-rest-beta) для поиска последней [схемы синхронизации](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta) каталога, чтобы синхронизировать объекты каталога, атрибуты и их типы с приложением.
- Используйте [политику развертывания функций](/graph/api/resources/featureRolloutPolicy?view=graph-rest-beta), чтобы помочь администраторам клиента выполнить пилотное развертывание функций для определенных групп перед включением их для всей организации.

### <a name="mail"></a>Почта
Используйте более детализированное разрешение приложений _Mail.ReadBasic.All_, чтобы читать почтовый ящик пользователя, кроме текста сообщений, текста предварительного просмотра, вложений и расширенных свойств, а также без возможности поиска в почтовом ящике. Теперь его можно применять в [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta) и [отслеживании изменений](delta-query-overview.md) для [сообщения](/graph/api/resources/message?view=graph-rest-beta) и объекта **mailFolder**.

### <a name="reports"></a>Отчеты
- Получите дополнительные [данные об использовании почтового ящика](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta) касательно числа и размера удаленных элементов.

### <a name="teamwork"></a>Командная работа
- [Устанавливайте](/graph/api/user-add-teamsappinstallation?view=graph-rest-beta), [удаляйте](/graph/api/user-delete-teamsappinstallation?view=graph-rest-beta), [обновляйте](/graph/api/user-upgrade-teamsappinstallation?view=graph-rest-beta) и [перечисляйте установленные приложения Microsoft Teams](/graph/api/user-list-teamsappinstallation?view=graph-rest-beta) для пользователя.
- Используйте доступ только для приложения, чтобы читать сообщения канала, а также отвечать на сообщения в каналах и беседах. [Запросите и получите утверждение](teams-protected-apis.md) для такого доступа.

## <a name="want-to-stay-in-the-loop"></a>Хотите получать актуальную информацию?
- Имеются ли сценарии, поддержку которых вы хотели бы видеть в Microsoft Graph? Предложите новые функции и проголосуйте за них на [Портале пользовательских приложений для Microsoft Graph](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests).
- Будьте активными участниками сообщества Microsoft Graph! [Присоединяйтесь](https://aka.ms/microsoftgraphcall) к ежемесячной видеоконференции сообщества Microsoft Graph.
- Зарегистрируйтесь в [программе для разработчиков Office 365](https://developer.microsoft.com/ru-RU/office/dev-program), получите бесплатную подписку на Office 365 и приступите к разработке!


## <a name="see-also"></a>См. также
- Периодически просматривайте [блог разработчиков Microsoft Graph](https://developer.microsoft.com/en-us/graph/blogs/), чтобы узнавать об объявленных выпусках и полезных ресурсах.
- Ознакомьтесь с подробными сведениями о дополнениях API Microsoft Graph и обновлениями действий API в [журнале изменений](changelog.md).
- Найдите [обзоры предыдущих выпусков](whats-new-earlier.md).
- Узнайте больше о [политиках в отношении управления версиями, поддержки и внесения критических изменений в Microsoft Graph](versioning-and-support.md).


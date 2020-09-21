---
title: Работа с API управления обслуживанием Azure AD
description: Управление доступом к ресурсам, в том числе группам, приложениям и сайтам с помощью управления правами Azure AD
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 7982cfd3cf167627879e2fe4d36e2f676b1ab16f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989530"
---
# <a name="working-with-the-azure-ad-entitlement-management-api"></a>Работа с API управления обслуживанием Azure AD

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Управление обслуживанием Azure Active Directory (Azure AD) помогает управлять доступом к группам, приложениям и сайтам SharePoint Online для внутренних пользователей, а также пользователей, не входящих в вашу организацию.

Создавайте пакеты Access с ролями, которые пользователи должны иметь в этих ресурсах, и определяя политики, которые могут запрашивать пакет Access и как долго они могут назначать доступ к пакету Access, можно управлять жизненным циклом доступа как для внутренних, так и для внешних пользователей.

Существуют следующие типы ресурсов управления обслуживанием.

- [акцесспаккаже](accesspackage.md): Определяет коллекции ролей ресурсов и политики того, как один или несколько пользователей могут получить доступ к этим ресурсам.
- [акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md): определяет политику, с помощью которой субъекты могут запрашивать или назначать пакет доступа с помощью назначения пакета Access.
- [акцесспаккажеассигнментрекуест](accesspackageassignmentrequest.md): создан пользователем, который хочет получить назначение пакета Access.
- [акцесспаккажеассигнмент](accesspackageassignment.md): назначение пакета доступа определенной теме в течение определенного периода времени.
- [акцесспаккажеассигнментресаурцероле](accesspackageassignmentresourcerole.md): Указывает роль, связанную с определенным ресурсом, которой назначена тема с помощью назначения пакета Access.
- [акцесспаккажекаталог](accesspackagecatalog.md): контейнер для пакетов доступа.
- [акцесспаккажересаурцерекуест](accesspackageresourcerequest.md): запрос на Добавление ресурса в каталог пакетов Access.
- [коннектедорганизатион](connectedorganization.md): подключенная организация для внешних пользователей, которые могут запрашивать доступ.
- [ентитлементманажементсеттингс](entitlementmanagementsettings.md): параметры на уровне клиента для управления обслуживанием Azure AD.

Руководство, в котором показано, как использовать управление обслуживанием для создания пакета ресурсов, которые внутренние пользователи могут использовать для самостоятельного запроса, в разделе [Создание пакета Access с помощью API Microsoft Graph](/graph/tutorial-access-package-api).

Обратите внимание, что функция управления обслуживанием, включая API, включена в Azure AD Premium P2. Клиент, на котором используется управление обслуживанием, должен иметь допустимую приобретенную или пробную подписку на Azure AD Premium P2 или EMS.

## <a name="methods"></a>Методы

В следующей таблице перечислены методы, которые можно использовать для взаимодействия с ресурсами, связанными с управлением ресурсами.

| Метод           | Тип возвращаемых данных    |Описание|
|:---------------|:--------|:----------|
| [получение](../api/entitlementmanagementsettings-get.md); | [ентитлементманажементсеттингс](entitlementmanagementsettings.md) | Чтение свойств объекта **ентитлементманажементсеттингс** . |
| [обновление](../api/entitlementmanagementsettings-update.md). | [ентитлементманажементсеттингс](entitlementmanagementsettings.md) | Обновление свойств объекта **ентитлементманажементсеттингс** . |
| [Список Акцесспаккажес](../api/accesspackage-list.md) | Коллекция [акцесспаккаже](accesspackage.md) | Получение списка объектов **акцесспаккаже** . |
| [Создание Акцесспаккаже](../api/accesspackage-post.md) | [акцесспаккаже](accesspackage.md) | Создание нового объекта **акцесспаккаже** . |
| [Получение Акцесспаккаже](../api/accesspackage-get.md) | [акцесспаккаже](accesspackage.md) | Чтение свойств и связей объекта **акцесспаккаже** . |
| [Обновление Акцесспаккаже](../api/accesspackage-update.md)|Нет | Обновление свойств объекта **акцесспаккаже** . |
| [Удаление Акцесспаккаже](../api/accesspackage-delete.md) | | Удаление **акцесспаккаже**. |
| [Список Акцесспаккажересаурцеролескопес](../api/accesspackage-list-accesspackageresourcerolescopes.md) | Коллекция [акцесспаккажересаурцеролескопе](accesspackageresourcerolescope.md) | Получение списка объектов **акцесспаккажересаурцеролескопе** для пакета Access. |
| [Создание Акцесспаккажересаурцеролескопе](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | Создайте новый объект **акцесспаккажересаурцеролескопе** для пакета Access. |
| [Список АкцесспаккажеассигнментполиЦиес](../api/accesspackageassignmentpolicy-list.md) | Коллекция [акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md) | Получение списка объектов **акцесспаккажеассигнментполици** . |
| [Создание Акцесспаккажеассигнментполици](../api/accesspackageassignmentpolicy-post.md) | [акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md)| Создание нового объекта **акцесспаккажеассигнментполици** . |
| [Получение Акцесспаккажеассигнментполици](../api/accesspackageassignmentpolicy-get.md) | [акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md) | Чтение свойств и связей объекта **акцесспаккажеассигнментполици** . |
| [Обновление Акцесспаккажеассигнментполици](../api/accesspackageassignmentpolicy-update.md)|[акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md) | Обновление свойств объекта **акцесспаккажеассигнментполици** . |
| [Удаление Акцесспаккажеассигнментполици](../api/accesspackageassignmentpolicy-delete.md) | | Удаление **акцесспаккажеассигнментполици**. |
| [Список Акцесспаккажеассигнментрекуестс](../api/accesspackageassignmentrequest-list.md) | Коллекция [акцесспаккажеассигнментрекуест](accesspackageassignmentrequest.md) | Получение списка объектов **акцесспаккажеассигнментрекуест** . |
| [Создание Акцесспаккажеассигнментрекуест](../api/accesspackageassignmentrequest-post.md) | [акцесспаккажеассигнментрекуест](accesspackageassignmentrequest.md) | Создание нового **акцесспаккажеассигнментрекуест**. |
| [Получение Акцесспаккажеассигнментрекуест](../api/accesspackageassignmentrequest-get.md) | [акцесспаккажеассигнментрекуест](accesspackageassignmentrequest.md) | Чтение свойств и связей объекта **акцесспаккажеассигнментрекуест** . |
| [Список Акцесспаккажеассигнментс](../api/accesspackageassignment-list.md) | Коллекция [акцесспаккажеассигнмент](accesspackageassignment.md) | Получение списка объектов **акцесспаккажеассигнмент** . |
| [Список Акцесспаккажеассигнментресаурцеролес](../api/accesspackageassignmentresourcerole-list.md) | Коллекция [акцесспаккажеассигнментресаурцероле](accesspackageassignmentresourcerole.md) | Получение списка объектов **акцесспаккажеассигнментресаурцероле** . |
| [Получение Акцесспаккажеассигнментресаурцероле](../api/accesspackageassignmentresourcerole-get.md) | [акцесспаккажеассигнментресаурцероле](accesspackageassignmentresourcerole.md)  | Получение объекта **акцесспаккажеассигнментресаурцероле** . |
| [Список Акцесспаккажекаталогс](../api/accesspackagecatalog-list.md) | Коллекция [акцесспаккажекаталог](accesspackagecatalog.md) | Получение списка объектов **акцесспаккажекаталогс** . |
| [Создание Акцесспаккажекаталог](../api/accesspackagecatalog-post.md) | [акцесспаккажекаталог](accesspackagecatalog.md) | Создание нового объекта **акцесспаккажекаталог** . |
| [Получение Акцесспаккажекаталог](../api/accesspackagecatalog-get.md) | [акцесспаккажекаталог](accesspackagecatalog.md) | Чтение свойств и связей объекта **акцесспаккажекаталог** . |
| [Обновление Акцесспаккажекаталог](../api/accesspackagecatalog-update.md)|Нет | Обновление свойств объекта **акцесспаккажекаталог** . |
| [Удаление Акцесспаккажекаталог](../api/accesspackagecatalog-delete.md) | | Удаление **акцесспаккажекаталог**. |
| [Список ресурсов Акцесспаккажекаталог](../api/accesspackagecatalog-list-accesspackageresources.md) | Коллекция [акцесспаккажересаурце](accesspackageresource.md) | Получение списка объектов **акцесспаккажересаурце** . |
| [Список ролей ресурсов Акцесспаккажекаталог](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | Коллекция [акцесспаккажересаурцероле](accesspackageresourcerole.md) | Получение списка объектов **акцесспаккажересаурцероле** . |
| [Список Акцесспаккажересаурцерекуестс](../api/accesspackageresourcerequest-list.md) | Коллекция [акцесспаккажересаурцерекуест](accesspackageresourcerequest.md) | Чтение свойств и связей объектов **акцесспаккажересаурцерекуест** . |
| [Создание Акцесспаккажересаурцерекуест](../api/accesspackageresourcerequest-post.md) | [акцесспаккажекаталог](accesspackageresourcerequest.md) | Создание нового объекта **акцесспаккажересаурцерекуест** . |
| [Список Коннектедорганизатионс](../api/connectedorganization-list.md) | Коллекция [коннектедорганизатион](connectedorganization.md) | Получение списка объектов **коннектедорганизатион** . |
| [Создание Коннектедорганизатион](../api/connectedorganization-post.md) | [коннектедорганизатион](connectedorganization.md) | Создание нового объекта **коннектедорганизатион** . |
| [Получение Коннектедорганизатион](../api/connectedorganization-get.md) | [коннектедорганизатион](connectedorganization.md) | Чтение свойств и связей объекта **коннектедорганизатион** . |
| [Обновление Коннектедорганизатион](../api/connectedorganization-update.md) |Нет | Обновление **коннектедорганизатион**. |
| [Удаление Коннектедорганизатион](../api/connectedorganization-delete.md) |Нет | Удаление объекта **коннектедорганизатион**. |
|[Список Интерналспонсорс](../api/connectedorganization-list-internalsponsors.md) | Коллекция [directoryObject](directoryobject.md) | Получение списка внутренних спонсоров **коннектедорганизатион** . |
|[Список Екстерналспонсорс](../api/connectedorganization-list-externalsponsors.md) | Коллекция [directoryObject](directoryobject.md) | Получение списка внешних спонсоров **коннектедорганизатион** . |
|[Добавление Интерналспонсорс](../api/connectedorganization-post-internalsponsors.md) | Нет | Добавление пользователя или группы в внутренние спонсоры **коннектедорганизатион** . |
|[Добавление Екстерналспонсорс](../api/connectedorganization-post-externalsponsors.md) | Нет | Добавление пользователя или группы во внешние спонсоры **коннектедорганизатион** . |
|[Удаление Интерналспонсорс](../api/connectedorganization-delete-internalsponsors.md) | Нет | Удаление пользователя или группы из внутренних спонсоров **коннектедорганизатион** . |
|[Удаление Екстерналспонсорс](../api/connectedorganization-delete-externalsponsors.md) | Нет | Удаление пользователя или группы из внешних спонсоров **коннектедорганизатион** . |

## <a name="types"></a>Типы

- [рекуесторсеттингс](requestorsettings.md), [аппровалсеттингс](approvalsettings.md) и [ассигнментревиевсеттингс](assignmentreviewsettings.md) — используется в [акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md) , чтобы указать, кто может запрашивать, кто утверждает и кто просматривает запросы на назначение пакетов для этой политики.
- [аппровалстаже](approvalstage.md) — используется в [аппровалсеттингс](approvalsettings.md) для указания основного, резервного и технического утверждающих лиц.
- [пользовательские](userset.md) подтипы [SingleUser.](singleuser.md), [граупмемберс](groupmembers.md), [коннектедорганизатионмемберс](connectedorganizationmembers.md), [рекуесторманажер](requestormanager.md), [интерналспонсорс](internalsponsors.md)и екстерналспонсорс используются в [externalSponsors](externalsponsors.md) [requestorSettings](requestorsettings.md), [approvalStage](approvalstage.md) и [assignmentReviewSettings](assignmentreviewsettings.md).
- [акцесспаккажесубжект](accesspackagesubject.md) — используется в [акцесспаккажеассигнмент](accesspackageassignment.md) в качестве пользователя темы с назначенным пакетом Access.
- [идентитисаурце](identitysource.md) — используется в [коннектедорганизатион](connectedorganization.md), один из [азуреактиведиректоритенант](azureactivedirectorytenant.md), [домаинидентитисаурце](domainidentitysource.md) или [externalDomainFederation](externaldomainfederation.md).

## <a name="see-also"></a>См. также

 - [Что такое управление обслуживанием Azure AD?](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-overview)



<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



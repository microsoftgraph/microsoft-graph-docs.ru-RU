---
title: Работа с API управления обслуживанием Azure AD
description: Управление доступом к ресурсам, в том числе группам, приложениям и сайтам с помощью управления правами Azure AD
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6eada39751a6ed107fb1b74d61100aa1a3469c83
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870290"
---
# <a name="working-with-the-azure-ad-entitlement-management-api"></a>Работа с API управления обслуживанием Azure AD

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Управление обслуживанием Azure Active Directory (Azure AD) помогает управлять доступом к группам, приложениям и сайтам SharePoint Online для внутренних пользователей, а также пользователей, не входящих в вашу организацию.

Создавайте пакеты Access с ролями, которые пользователи должны иметь в этих ресурсах, и определяя политики, которые могут запрашивать пакет Access и как долго они могут назначить пакет Access, можно управлять жизненным циклом доступа как для внутренних, так и для внешние пользователи.

Существуют следующие типы ресурсов управления обслуживанием.

- [акцесспаккаже](accesspackage.md): Определяет коллекции ролей ресурсов и политики того, как один или несколько пользователей могут получить доступ к этим ресурсам.
- [акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md): определяет политику, с помощью которой субъекты могут запрашивать или назначать пакет доступа с помощью назначения пакета Access.
- [акцесспаккажеассигнментрекуест](accesspackageassignmentrequest.md): создан пользователем, который хочет получить назначение пакета Access.
- [акцесспаккажеассигнмент](accesspackageassignment.md): назначение пакета доступа определенной теме в течение определенного периода времени.
- [акцесспаккажеассигнментресаурцероле](accesspackageassignmentresourcerole.md): Указывает роль, связанную с определенным ресурсом, которой назначена тема с помощью назначения пакета Access.
- [акцесспаккажекаталог](accesspackagecatalog.md): контейнер для пакетов доступа.
- [акцесспаккажересаурцерекуест](accesspackageresourcerequest.md): запрос на Добавление ресурса в каталог пакетов Access.

Обратите внимание, что функция управления обслуживанием, включая API, включена в Azure AD Premium P2. Клиент, на котором используется управление обслуживанием, должен иметь допустимую приобретенную или пробную подписку на Azure AD Premium P2 или EMS.

## <a name="methods"></a>Methods

В следующей таблице перечислены методы, которые можно использовать для взаимодействия с ресурсами, связанными с управлением ресурсами.

| Метод           | Тип возвращаемых данных    |Описание|
|:---------------|:--------|:----------|
| [Список Акцесспаккажес](../api/accesspackage-list.md) | Коллекция [акцесспаккаже](accesspackage.md) | Получение списка объектов **акцесспаккаже** . |
| [Создание Акцесспаккаже](../api/accesspackage-post.md) | [акцесспаккаже](accesspackage.md) | Создание нового объекта **акцесспаккаже** . |
| [Получение Акцесспаккаже](../api/accesspackage-get.md) | [акцесспаккаже](accesspackage.md) | Чтение свойств и связей объекта **акцесспаккаже** . |
| [Удаление Акцесспаккаже](../api/accesspackage-delete.md) | | Удаление **акцесспаккаже**. |
| [Список Акцесспаккажересаурцеролескопес](../api/accesspackage-list-accesspackageresourcerolescopes.md) | Коллекция [акцесспаккажересаурцеролескопе](accesspackageresourcerolescope.md) | Получение списка объектов **акцесспаккажересаурцеролескопе** для пакета Access. |
| [Создание Акцесспаккажересаурцеролескопе](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | Создайте новый объект **акцесспаккажересаурцеролескопе** для пакета Access. |
| [Список АкцесспаккажеассигнментполиЦиес](../api/accesspackageassignmentpolicy-list.md) | Коллекция [акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md) | Получение списка объектов **акцесспаккажеассигнментполици** . |
| [Создание Акцесспаккажеассигнментполици](../api/accesspackageassignmentpolicy-post.md) | [акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md)| Создание нового объекта **акцесспаккажеассигнментполици** . |
| [Получение Акцесспаккажеассигнментполици](../api/accesspackageassignmentpolicy-get.md) | [акцесспаккажеассигнментполици](accesspackageassignmentpolicy.md) | Чтение свойств и связей объекта **акцесспаккажеассигнментполици** . |
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
| [Удаление Акцесспаккажекаталог](../api/accesspackagecatalog-delete.md) | | Удаление **акцесспаккажекаталог**. |
| [Список ресурсов Акцесспаккажекаталог](../api/accesspackagecatalog-list-accesspackageresources.md) | Коллекция [акцесспаккажересаурце](accesspackageresource.md) | Получение списка объектов **акцесспаккажересаурце** . |
| [Список ролей ресурсов Акцесспаккажекаталог](../api/accesspackagecatalog-list-accesspackageresourceroles.md) | Коллекция [акцесспаккажересаурцероле](accesspackageresourcerole.md) | Получение списка объектов **акцесспаккажересаурцероле** . |
| [Список Акцесспаккажересаурцерекуестс](../api/accesspackageresourcerequest-list.md) | Коллекция [акцесспаккажересаурцерекуест](accesspackageresourcerequest.md) | Чтение свойств и связей объектов **акцесспаккажересаурцерекуест** . |
| [Создание Акцесспаккажересаурцерекуест](../api/accesspackageresourcerequest-post.md) | [акцесспаккажекаталог](accesspackageresourcerequest.md) | Создание нового объекта **акцесспаккажересаурцерекуест** . |

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

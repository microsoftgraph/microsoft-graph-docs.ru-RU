---
title: Тип ресурса administrativeUnit
description: Административное устройство предоставляет концептуальный контейнер для объектов каталога пользователей и групп.
localization_priority: Normal
author: anandyadavMSFT
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e97ca2eba834931e311c3f10b85991697d66360b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059558"
---
# <a name="administrativeunit-resource-type"></a>Тип ресурса administrativeUnit

Пространство имен: microsoft.graph

Административное устройство предоставляет концептуальный контейнер для объектов каталога пользователей и групп. С помощью административных единиц администратор компании может делегировать административные обязанности для управления пользователями и группами, которые находятся в административной единице или в области действия, на региональном или подразделенном администраторе.

Рассмотрим эти действия на примере. Представьте, что компания Contoso Corp состоит из двух подразделений — западных и восточноазиатских подразделений. Роли каталога в компании Contoso ограничены всеми клиентами. Иванов, администратор компании Contoso, хочет делегировать административные обязанности, а область их до деления Западного или Восточного Дальневосточный.  Пользователь может создать *единицу измерения "Западный адмистративе* " и поместить все пользователи с Западом Дальневосточный в эту административную единицу.  Аналогичным образом, Иванов может создать *админстративе единицу Восточной побережье*.  Теперь можно приступить к делегированию административных обязанностей другим пользователям, но с **областью действия** , созданной для новых административных модулей, которые он создал. Иванов помещает Jennifer в роль *администратора службы поддержки* в **область** *административное подразделение Дальневосточный Запад*.  Это позволяет Jennifer сбросить пароль любого пользователя, но только в том случае, если эти пользователи находятся в *административном подразделении Дальневосточный Запад*.  Аналогичным образом, Иванову помещаете Дениса в роль *администратора учетных записей пользователей* с **областью** *административного подразделения East Дальневосточный*.  Это позволяет Дениса обновлять пользователей, назначать лицензии и сбрасывать пароли всех пользователей, но только если они находятся в *административном модуле "Восток*". Для просмотра видео ознакомьтесь со статьей [Введение в административные единицы Azure Active Directory](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units).


В этом разделе описаны объявленные свойства и свойства навигации, предоставляемые объектом administrativeUnit, а также операции и функции, которые можно вызывать для ресурса Административеунитс.


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Создание](../api/administrativeunit-post-administrativeunits.md) | [administrativeUnit](administrativeunit.md) | Создайте новое административное подразделение.|
|[List](../api/administrativeunit-list.md) | Коллекция [administrativeUnit](administrativeunit.md) |Список свойств всех Административеунитс.|
|[получение](../api/administrativeunit-get.md); | [administrativeUnit](administrativeunit.md) |Чтение свойств и связей определенного объекта administrativeUnit.|
|[обновление](../api/administrativeunit-update.md). | [administrativeUnit](administrativeunit.md)    |Обновление объекта administrativeUnit. |
|[удаление](../api/administrativeunit-delete.md); | Нет |Удаление объекта administrativeUnit. |
|[Добавить участника](../api/administrativeunit-post-members.md) |[directoryObject](directoryobject.md)| Добавление члена (пользователя или группы).|
|[Перечисление участников](../api/administrativeunit-list-members.md) |Коллекция [directoryObject](directoryobject.md)| Получение списка участников (пользователей и групп).|
|[Получение члена](../api/administrativeunit-get-members.md) |[directoryObject](directoryobject.md)| Получение определенного участника.|
|[Удаление члена](../api/administrativeunit-delete-members.md) |[directoryObject](directoryobject.md)| Удаление члена.|
|[Добавление роли члена с областью](../api/administrativeunit-post-scopedrolemembers.md) |[Scopedrolemembership изменен](scopedrolemembership.md)| Добавление члена с областью ролей.|
|[Область списка — элементы роли](../api/administrativeunit-list-scopedrolemembers.md) |Коллекция [scopedRoleMembership](scopedrolemembership.md)| Получение списка администраторов ролей с областью действия.|
|[Получение члена роли с областью действия](../api/administrativeunit-get-scopedrolemembers.md) |[Scopedrolemembership изменен](scopedrolemembership.md)| Получение определенного члена с областью действия роли.|
|[Удаление члена с областью ролей](../api/administrativeunit-delete-scopedrolemembers.md) |[Scopedrolemembership изменен](scopedrolemembership.md)| Удаление члена с областью ролей.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|description|string|Необязательное описание административной единицы.|
|displayName|string|Отображаемое имя административной единицы.|
|id|string|Уникальный идентификатор административной единицы. Только для чтения.|
|visibility|string|Определяет, является ли модуль админстративе и его элементы скрытыми или общедоступными. Может быть задано значение значение hiddenmembership или public. Если не задано, то поведение по умолчанию — Public. Если задано значение значение hiddenmembership, только члены административной единицы могут перечислить других членов единицы админстративе.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|members|Коллекция [directoryObject](directoryobject.md)|Пользователи и группы, являющиеся членами этого Админситративе подразделения. Методы HTTP: GET (List Members), POST (Add Members), DELETE (удалить участников).|
|Scopedadministrators|Коллекция [scopedRoleMembership](scopedrolemembership.md)| Члены роли с областью действия этой административной единицы.  Методы HTTP: GET (List Скопедролемембершипс), POST (Add Scopedrolemembership изменен), DELETE (удалить Scopedrolemembership изменен). |

## <a name="json-representation"></a>Представление JSON

Ниже показано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.administrativeUnit"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "visibility": "string"
}

```


## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users)
- [Добавление пользовательских данных в группы с помощью расширений схемы](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "administrativeUnit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

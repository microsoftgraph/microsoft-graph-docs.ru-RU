---
title: Тип ресурса administrativeUnit
description: Административная единица предоставляет концептуальный контейнер для объектов каталога пользователей, групп и устройств.
ms.localizationpriority: medium
author: DougKirschner
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 40f81892de0fe1a9925a6d9d62d51e679b57748b
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899465"
---
# <a name="administrativeunit-resource-type"></a>Тип ресурса administrativeUnit

Пространство имен: microsoft.graph

Административная единица предоставляет концептуальный контейнер для объектов каталога пользователей, групп и устройств. С помощью административных единиц администратор компании теперь может делегировать административные обязанности по управлению пользователями, группами и устройствами, содержащимся в административной единице или в области действия, региональным администраторам или администраторам отделов. Этот ресурс относится к открытому типу, который позволяет передавать другие свойства.

Рассмотрим эти действия на примере. Представьте себе, что компания Contoso состоит из двух подразделений: западно-западного и восточно-западного. Роли каталога в Contoso применяются ко всему клиенту. Ли, администратор компании Contoso, хочет делегировать административные обязанности, но ограничить их в западно-приморском или восточном побережье.  Ли может создать *административную* единицу западного побережья и поместить всех пользователей западного побережья в эту административную единицу.  Аналогичным образом Ли может создать административное *подразделение "Восточная часть Приморья"*.  Теперь Ли может приступить к делегированию административных обязанностей  другим пользователям, но областью действия будут новые административные единицы, которые он создал. Ли помещает Его в роль *администратора службы* технической поддержки, **областью** действия является *административная единица "Западная побереговая"*.  Это позволяет Пользователю сбросить пароль любого пользователя, но только в том случае, если эти пользователи находятся в административной единице " *Западная часть Сша"*.  Аналогичным образом Ли помещает Дэвида в роль  администратора учетной записи пользователя **, областью** действия является *административная единица "Восточная поберегов"*.  Это позволяет Пользователю обновлять пользователей, назначать лицензии и сбрасывать пароль любого пользователя, но только в том случае, если эти пользователи находятся в административной единице "Восточная *часть"*. Обзор видео см. в статье " [Общие сведения об административных единицах Azure Active Directory"](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units).


В этом разделе приводятся описания объявленных свойств и свойств навигации, предоставляемых сущностью administrativeUnit, а также операций и функций, которые могут быть вызваны в ресурсе administrativeUnits.


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Создание](../api/directory-post-administrativeunits.md) | [administrativeUnit](administrativeunit.md) | Создайте новую административную единицу.|
|[Список](../api/directory-list-administrativeunits.md) | [Коллекция administrativeUnit](administrativeunit.md) |Список свойств всех объектов administrativeUnits.|
|[Get](../api/administrativeunit-get.md) | [administrativeUnit](administrativeunit.md) |Чтение свойств и связей определенного объекта administrativeUnit.|
|[Обновление](../api/administrativeunit-update.md) | [administrativeUnit](administrativeunit.md)    |Обновление объекта administrativeUnit. |
|[Удаление](../api/administrativeunit-delete.md) | Нет |Удаление объекта administrativeUnit. |
|[Добавить участника](../api/administrativeunit-post-members.md) |[directoryObject](directoryobject.md)| Добавьте участника (пользователя, группу или устройство).|
|[Перечисление участников](../api/administrativeunit-list-members.md) |Коллекция [directoryObject](directoryobject.md)| Получение списка участников (пользователя, группы или устройства).|
|[Получение члена](../api/administrativeunit-get-members.md) |[directoryObject](directoryobject.md)| Получение определенного члена.|
|[Удаление члена](../api/administrativeunit-delete-members.md) |[directoryObject](directoryobject.md)| Удалите член.|
|[Добавление scopedRoleMember](../api/administrativeunit-post-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Назначьте роль Azure AD с областью административной единицы.|
|[Перечисление scopedRoleMembers](../api/administrativeunit-list-scopedrolemembers.md) |Коллекция [scopedRoleMembership](scopedrolemembership.md)| Вывод списка назначений ролей Azure AD с областью административной единицы.|
|[Получение объекта scopedRoleMember](../api/administrativeunit-get-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Получение назначения роли Azure AD с областью административной единицы.|
|[Удаление объекта scopedRoleMember](../api/administrativeunit-delete-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Удаление назначения роли Azure AD с областью административной единицы.|

## <a name="properties"></a>Свойства

> [!IMPORTANT]
> Определенное использование `$filter` и параметра запроса `$search` поддерживается только при применении заголовка **ConsistencyLevel** с присвоенным значением `eventual` и `$count`. Дополнительные сведения см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries#administrative-unit-properties).

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|description|Строка|Необязательное описание административной единицы. `$filter` Поддерживает (`eq`, `ne`, `in`, `startsWith`), `$search`.|
|displayName|Строка|Отображаемое имя административной единицы. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` для значений `null`), `$search` и `$orderBy`.|
|id|Строка|Уникальный идентификатор административной единицы. Только для чтения. Поддерживает `$filter` (`eq`).|
|visibility|String|Определяет, скрыта ли административная единица и ее члены. Можно задать значение `HiddenMembership`.. Если не задано (значение равно `null`), поведение по умолчанию является общедоступным. Если задано значение `HiddenMembership`,только члены административной единицы могут выведите список других членов административной единицы.|

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|extensions|Коллекция объектов [extension](extension.md)|Коллекция открытых расширений, определенных для этой административной единицы. Допускается значение null.|
|members|Коллекция [directoryObject](directoryobject.md)|Пользователи и группы, которые являются членами этой административной единицы. Поддерживает `$expand`.|
|scopedRoleMembers|Коллекция [scopedRoleMembership](scopedrolemembership.md)| Элементы с заданной областью роли этой административной единицы. |

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
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "visibility": "String"
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

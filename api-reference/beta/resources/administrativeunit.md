---
title: тип ресурса administrativeUnit
description: Административное подразделение предоставляет концептуальный контейнер для объектов каталогов пользователей и групп.
ms.localizationpriority: medium
author: DougKirschner
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 5f689a44f614d7eb263d5d24fbaae6b7c7998543
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854750"
---
# <a name="administrativeunit-resource-type"></a>тип ресурса administrativeUnit

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Административное подразделение предоставляет концептуальный контейнер для объектов каталогов пользователей и групп. С помощью административных подразделений администратор компании теперь может делегировать административные обязанности по управлению пользователями и группами, содержамися в пределах или в пределах области, административному подразделению региональному или ведомству.

Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/administrativeunit-delta.md). Этот ресурс относится к открытому типу, который позволяет передавать другие свойства.

Рассмотрим эти действия на примере. Imagine, что Contoso Corp состоит из двух подразделений — подразделения Западного побережья и подразделения Восточного побережья. Роли каталога в Contoso имеют область действия для всего клиента. Ли, администратор компании Contoso, хочет делегировать административные обязанности, но область их в отдел Западного побережья или подразделение Восточного побережья.  Ли может создать адмистративный блок *Западного* побережья и разместить всех пользователей западного побережья в это административное подразделение.  Кроме того, Ли может создать админстративную единицу *Восточного побережья*.  Теперь Ли может начать делегирование административных обязанностей другим, но в  области новых созданных им административных подразделений. Ли помещает Дженнифер в *роль администратора helpdesk***, которая имеет область действия** для административного *подразделения Западного побережья*.  Это позволяет Дженнифер сбросить пароль любого пользователя, но только в том случае, если эти пользователи находятся в административном подразделении *Западного побережья*.  Кроме того, Ли помещает Дэйва *в роль* администратора учетной записи пользователя **, которая имеет** область действия для *административного подразделения Восточного побережья*.  Это позволяет Дэйву обновлять пользователей, назначать лицензии и сбрасывать пароль любого пользователя, но только в том случае, если эти пользователи находятся в административном подразделении *Восточного побережья*. Обзор видео см. в обзоре [Введение в Azure Active Directory административных единиц](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units).

С помощью этого ресурса можно добавлять собственные данные к настраиваемым свойствам, применяя [расширения](/graph/extensibility-overview).

В этом разделе описаны заявленные свойства и свойства навигации, выставленные объектом administrativeUnit, а также операции и функции, которые можно назвать на ресурсе administrativeUnits.


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Создание](../api/directory-post-administrativeunits.md) | [administrativeUnit](administrativeunit.md) | Создание нового административного подразделения.|
|[Список](../api/directory-list-administrativeunits.md) | [коллекция administrativeUnit](administrativeunit.md) |Список свойств всех административных объектов.|
|[Получение](../api/administrativeunit-get.md); | [administrativeUnit](administrativeunit.md) |Чтение свойств и связей определенного объекта administrativeUnit.|
|[Обновление](../api/administrativeunit-update.md) | [administrativeUnit](administrativeunit.md)    |Обновление объекта administrativeUnit. |
|[удаление](../api/administrativeunit-delete.md); | Нет |Удаление объекта administrativeUnit. |
|[Получение дельты](../api/administrativeunit-delta.md)|[administrativeUnit](administrativeunit.md)|Создайте заново созданные, обновленные или удаленные **административные** подразделения, не выполняя полное чтение всей коллекции ресурсов.|
|[Добавить участника](../api/administrativeunit-post-members.md) |[directoryObject](directoryobject.md)| Добавление участника (пользователя или группы).|
|[Перечисление участников](../api/administrativeunit-list-members.md) |Коллекция [directoryObject](directoryobject.md)| Получите список участников (пользователей и групп).|
|[Получение члена](../api/administrativeunit-get-members.md) |[directoryObject](directoryobject.md)| Получите определенного участника.|
|[Удаление члена](../api/administrativeunit-delete-members.md) |[directoryObject](directoryobject.md)| Удалите член.|
|[Добавление члена scoped-role](../api/administrativeunit-post-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Добавление члена с областью действия роли.|
|[Участники списка с областью ролей](../api/administrativeunit-list-scopedrolemembers.md) |Коллекция [scopedRoleMembership](scopedrolemembership.md)| Получите список администраторов с масштабной ролью.|
|[Получить участника с областью действия](../api/administrativeunit-get-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Получите определенного члена с областью действия.|
|[Удаление члена с областью ролей](../api/administrativeunit-delete-scopedrolemembers.md) |[scopedRoleMembership](scopedrolemembership.md)| Удаление члена с областью действия.|
|**Открытые расширения**| | |
|[Создание открытого расширения](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Создание открытого расширения и добавление настраиваемых свойств в новый или существующий ресурс.|
|[Получение открытого расширения](../api/opentypeextension-get.md) |Коллекция объектов [openTypeExtension](opentypeextension.md)| Получение открытого расширения, определяемого именем расширения.|
|**Расширения схемы**| | |
|[Добавление значений расширений для схемы](/graph/extensibility-schema-groups) || Создание определения расширения схемы и его дальнейшее использование для добавления в ресурс введенных пользовательских данных.|

> [!NOTE]
> Конечная точка URL-адреса для вызова API **administrativeUnits** находится `/administrativeUnits` `beta` в конечной точке, но `/directory/administrativeUnits` в конечной `v1.0` точке.

## <a name="properties"></a>Свойства

> [!IMPORTANT]
> Определенное использование `$filter` и параметра запроса `$search` поддерживается только при применении заголовка **ConsistencyLevel** с присвоенным значением `eventual` и `$count`. Дополнительные сведения см. в статье [Расширенные возможности запросов для объектов каталога Azure AD](/graph/aad-advanced-queries#administrative-unit-properties).

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|description|String|Необязательное описание административного подразделения. `$filter` Поддерживает (`eq`, `ne`, `in`, ), `startsWith``$search`.|
|displayName|Строка|Отображение имени административного подразделения. Поддерживает `$filter` (`eq`, `ne`, `not`, `ge`, `le`, `in`, `startsWith` и `eq` по `null` значениям), `$search` и `$orderBy`.|
|id|String|Уникальный идентификатор для административного подразделения. Только для чтения. Поддерживает `$filter` (`eq`).|
|visibility|String|Контролирует, скрыта ли административная единица и ее члены. Можно установить .`HiddenMembership` Если не установлено (значение есть `null`), поведение по умолчанию является общедоступным. При наборе `HiddenMembership`только члены административного подразделения могут перечислять других членов административного подразделения.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для этого административного подразделения. Допускается значение null.|
|members|Коллекция [directoryObject](directoryobject.md)|Пользователи и группы, которые являются членами этого административного подразделения. Поддерживает `$expand`.|
|scopedRoleMembers|Коллекция [scopedRoleMembership](scopedrolemembership.md)| Члены этого административного подразделения с масштабной ролью.|

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



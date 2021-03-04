---
title: тип ресурса administrativeUnit
description: Административное подразделение предоставляет концептуальный контейнер для объектов каталогов пользователей и групп.
localization_priority: Normal
author: anandyadavMSFT
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 251aa5113e6ebd20b4f58f4cde340dbfbbd3d2ce
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433238"
---
# <a name="administrativeunit-resource-type"></a>тип ресурса administrativeUnit

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Административное подразделение предоставляет концептуальный контейнер для объектов каталогов пользователей и групп. С помощью административных подразделений администратор компании теперь может делегировать административные обязанности по управлению пользователями и группами, содержамися в пределах или в пределах области, административному подразделению региональному или ведомству.

Этот ресурс поддерживает отслеживание добавлений, удалений и обновлений с помощью [разностного запроса](/graph/delta-query-overview) с функцией [delta](../api/administrativeunit-delta.md).

Рассмотрим эти действия на примере. Представьте себе, что Contoso Corp состоит из двух подразделений — подразделения Западного побережья и подразделения Восточного побережья. Роли каталога в Contoso имеют область действия для всего клиента. Ли, администратор компании Contoso, хочет делегировать административные обязанности, но область их в отдел Западного побережья или подразделение Восточного побережья.  Ли может создать адмистративный блок *Западного* побережья и разместить всех пользователей западного побережья в это административное подразделение.  Кроме того, Ли может создать админстративную единицу *Восточного побережья.*  Теперь Ли может начать делегирование административных  обязанностей другим, но в области новых созданных им административных подразделений. Ли помещает Дженнифер в *роль администратора helpdesk,* **которая имеется** в административном подразделении *Западного побережья.*  Это позволяет Дженнифер сбросить пароль любого пользователя, но только в том случае, если эти пользователи находятся в административном подразделении *Западного побережья.*  Кроме того, Ли помещает Дэйва *в* роль администратора учетной записи пользователя, которая **имеет** область охвата *административного подразделения Восточного побережья.*  Это позволяет Дэйву обновлять пользователей, назначать лицензии и сбрасывать пароль любого пользователя, но только в том случае, если эти пользователи находятся в административном подразделении *Восточного побережья.* Обзор видео см. в обзоре Введение в административные единицы [Azure Active Directory.](https://channel9.msdn.com/Series/Windows-Azure-Active-Directory/Introduction-to-Azure-Active-Directory-Administrative-Units)

С помощью этого ресурса можно добавлять собственные данные к настраиваемым свойствам, применяя [расширения](/graph/extensibility-overview).

В этом разделе описаны заявленные свойства и свойства навигации, выставленные объектом administrativeUnit, а также операции и функции, которые можно назвать на ресурсе administrativeUnits.


## <a name="methods"></a>Методы

| Метод   | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Создание](../api/administrativeunit-post-administrativeunits.md) | [administrativeUnit](administrativeunit.md) | Создание нового административного подразделения.|
|[List](../api/administrativeunit-list.md) | [коллекция administrativeUnit](administrativeunit.md) |Список свойств всех административных объектов.|
|[получение](../api/administrativeunit-get.md); | [administrativeUnit](administrativeunit.md) |Чтение свойств и связей определенного объекта administrativeUnit.|
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

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|description|string|Необязательное описание административного подразделения.|
|displayName|string|Отображение имени административного подразделения.|
|id|string|Уникальный идентификатор для административного подразделения. Только для чтения.|
|visibility|string|Контролирует, скрыта ли админстративная единица и ее члены. Можно установить в HiddenMembership или Public. Если не установлено, поведение по умолчанию является общедоступным. При наборе к HiddenMembership только члены административного подразделения могут перечислять других членов админстративного подразделения.|

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|extensions|Коллекция [extension](extension.md)|Коллекция открытых расширений, определенных для этого административного подразделения. Допускается значение null.|
|members|Коллекция [directoryObject](directoryobject.md)|Пользователи и группы, которые являются членами этого администраторского подразделения. МЕТОДЫ HTTP: GET (участники списка), POST (добавление участников), DELETE (удаление участников).|
|scopedRoleMembers|Коллекция [scopedRoleMembership](scopedrolemembership.md)| Scoped-role members of this Administrative Unit.  МЕТОДЫ HTTP: GET (список scopedRoleMemberships), POST (добавление scopedRoleMembership), DELETE (remove scopedRoleMembership). |

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



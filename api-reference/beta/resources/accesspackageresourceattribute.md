---
title: тип ресурса accessPackageResourceAttribute
description: Ресурс, который предоставляет свойства для запрашивателя пакета доступа для предоставления настраиваемой информации, которая может быть использована для принятия решений об утверждении пакета доступа.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 27fdb3e5cf90b3a4a7d691b2c44c1d8b36a7d9ab
ms.sourcegitcommit: 2d61a35735aeb060cc9f7374dd6b50900566293b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2022
ms.locfileid: "62468301"
---
# <a name="accesspackageresourceattribute-resource-type"></a>тип ресурса accessPackageResourceAttribute

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Атрибут ресурса пакета доступа — это определение свойства, необходимого пользователю для доступа к приложению. Эта структура включена в [accessPackageResource](../resources/accesspackageresource.md) каталога для приложения, роли которого включены в пакет доступа в этом каталоге. Когда пользователь запрашивает пакет доступа, он должен предоставить значение атрибута, который, если запрос будет одобрен, затем записан на объекте каталога пользователя. Затем приложение может [считыть атрибут пользователя](../api/user-get.md).


## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|attributeDestination|[accessPackageResourceAttributeDestination](../resources/accesspackageresourceattributedestination.md)|Сведения о том, как установить атрибут, в настоящее время [тип объекта accessPackageUserDirectoryAttributeStore](accesspackageuserdirectoryattributestore.md) .|
|attributeName|Строка|Имя атрибута в конечной системе. Если предназначено, `accessPackageUserDirectoryAttributeStore`то свойство пользователя, например **jobTitle** или расширение схемы каталога для типа объекта пользователя, `extension_2b676109c7c74ae2b41549205f1947ed_personalTitle`например . |
|attributeSource|[accessPackageResourceAttributeSource](../resources/accesspackageresourceattributesource.md)|Сведения о том, как заполнить значение атрибута при выполнении **accessPackageAssignmentRequest** , в настоящее время тип [объекта accessPackageResourceAttributeQuestion](accesspackageresourceattributequestion.md) .|
|id|Строка|Уникальный идентификатор атрибута на ресурсе пакета доступа. Только для чтения. |
|isEditable|Строка| Указывает, может ли запрашиватель изменить существующее значение атрибута.|
|isPersistedOnAssignmentRemoval|Логический| Указывает, останется ли атрибут в конечном системе после окончания назначения.|


### <a name="accesspackageresourceattribute-resource-type-and-extension-properties"></a>свойства и свойства ресурсов accessPackageResourceAttribute

Свойства **attributeDestination**, **attributeName** и **attributeSource** атрибута ресурса пакета доступа относятся к свойствам расширения [каталога](extensionproperty.md).

Если **атрибутDestination** — это тип [объекта accessPackageUserDirectoryAttributeStore](accesspackageuserdirectoryattributestore.md), атрибут, указанный **атрибутом AttributeName**, должен быть обязательным свойством [объекта пользователя.](user.md) Эти свойства являются типами строк, зарегистрированными в качестве свойств [расширения](extensionproperty.md) на объекте **целевого** пользователя.

Например, предположим, что приложению требуется два атрибута пользователя, название задания пользователя и его личное название. Значения этих атрибутов можно синхронизировать с Azure AD из локального задания Active **DirectoryTitle** и **personalTitle** . Поскольку **personalTitle** не является одним из свойств объекта пользователя по умолчанию, [](user.md) для добавления свойства **personalTitle** в тип объекта пользователя потребуется создать расширение схемы каталога.[](../api/application-post-extensionproperty.md) При создании запроса ресурсов для приложения можно включить два атрибута ресурса пакета доступа: один для свойства пользователя **jobTitle** и другой с именем свойства расширения схемы каталога, созданного для личного заголовка, `extension_2b676109c7c74ae2b41549205f1947ed_personalTitle`например .

Если **атрибутОм** атрибута является [accessPackageResourceAttributeQuestion](accesspackageresourceattributequestion.md), то предоставленное значение запросителя хранится в соответствии с предоставленным объектом пользователя и предоставляется приложению и другим клиентам Microsoft Graph.
## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageResourceAttribute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceAttribute",
  "attributeDestination": {
    "@odata.type": "microsoft.graph.accessPackageResourceAttributeDestination"
  },
  "attributeName": "String",
  "attributeSource": {
    "@odata.type": "microsoft.graph.accessPackageResourceAttributeSource"
  },
  "id": "String (identifier)",
  "isEditable": "Boolean",
  "isPersistedOnAssignmentRemoval": "Boolean"
}
```

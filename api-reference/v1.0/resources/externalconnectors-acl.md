---
title: тип ресурса acl
description: Запись элемента управления доступом для элемента, индексного Поиск (Майкрософт) externalConnection.
author: mecampos
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 523ce420b4796d6ca3032839bf28393ea4975d21
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123491"
---
# <a name="acl-resource-type"></a>тип ресурса acl

Пространство имен: microsoft.graph.externalConnectors

Запись элемента управления доступом для элемента, индексного Поиск (Майкрософт) externalConnection.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|accessType|microsoft.graph.externalConnectors.accessType|Доступ, предоставленный удостоверению. Возможные значения: `grant`, `deny`, `unknownFutureValue`.|
|type|microsoft.graph.externalConnectors.aclType|Тип удостоверения. Возможные значения: `user`, `group`, `everyone`, `everyoneExceptGuests`, `externalGroup`, `unknownFutureValue`.|
|value|String|Уникальный идентификатор удостоверения. В случае Azure Active Directory удостоверений устанавливается идентификатор объекта пользователя, группы или клиента для пользователей, групп и всех `value` (и всех пользователейExceptGuests) соответственно. Если внешние группы `value` задают ID externalGroup |

## <a name="relationships"></a>Отношения
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.acl"
}
-->
``` json
{
  "type": "String",
  "value": "String",
  "accessType": "String"
}
```


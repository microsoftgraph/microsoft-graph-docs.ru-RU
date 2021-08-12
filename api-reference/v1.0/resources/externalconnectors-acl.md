---
title: тип ресурса acl
description: Запись элемента управления доступом для элемента, индексного Поиск (Майкрософт) externalConnection.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 56fa0c8f47f9bec9e2c00cbff3423a8aed541a2709c117326d3d0a29effabc08
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141695"
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

## <a name="relationships"></a>Связи
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


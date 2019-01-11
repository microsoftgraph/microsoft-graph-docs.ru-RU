---
title: Тип ресурса mimeContent
description: Содержит свойства обычного содержимого MIME.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 826606d41feb0f0a156a1b8240bde7f4ac926a5a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838229"
---
# <a name="mimecontent-resource-type"></a>Тип ресурса mimeContent

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства обычного содержимого MIME.
## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|type|Строка|Указывает MIME-тип содержимого.|
|value|Binary|Массив байтов содержимого.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mimeContent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mimeContent",
  "type": "String",
  "value": "binary"
}
```






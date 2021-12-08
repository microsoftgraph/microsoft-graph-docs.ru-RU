---
title: Тип ресурса удостоверений
description: Удостоверение
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b689afec67cae4b0c228d1a3ee96498a87a2548e
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346775"
---
# <a name="identity-resource-type"></a>Тип ресурса удостоверений

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Удостоверение

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор удостоверения. Это свойство доступно только для чтения.|
|displayName|Строка|Отображение имени удостоверения. Это свойство доступно только для чтения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identity",
  "id": "String (identifier)",
  "displayName": "String"
}
```





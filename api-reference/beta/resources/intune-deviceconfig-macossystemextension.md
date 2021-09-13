---
title: тип ресурса macOSSystemExtension
description: Представляет определенное расширение системы macOS.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7d88b72d155a6d83757befe30c83a0c1c941c788
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59106156"
---
# <a name="macossystemextension-resource-type"></a>тип ресурса macOSSystemExtension

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет определенное расширение системы macOS.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|teamIdentifier|String|Получает или задает идентификатор группы, который использовался для подписи расширения системы.|
|bundleId|String|Получает или задает идентификатор пакета расширения системы.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSSystemExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSystemExtension",
  "teamIdentifier": "String",
  "bundleId": "String"
}
```




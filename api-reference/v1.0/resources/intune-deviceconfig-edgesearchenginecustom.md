---
title: Тип ресурса edgeSearchEngineCustom
description: Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 367c81764bbf54cef8e5645c08fcb93ec430518d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028331"
---
# <a name="edgesearchenginecustom-resource-type"></a>Тип ресурса edgeSearchEngineCustom

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.


Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|edgeSearchEngineOpenSearchXmlUrl|String|Указывает на HTTPS-ссылку, содержащую XML-файл OpenSearch, в котором указаны по крайней мере краткое имя и URL-адрес поисковой системы.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineCustom",
  "edgeSearchEngineOpenSearchXmlUrl": "String"
}
```




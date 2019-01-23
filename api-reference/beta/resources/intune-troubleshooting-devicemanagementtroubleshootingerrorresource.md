---
title: Тип ресурса deviceManagementTroubleshootingErrorResource
description: Объект, представляющий ссылку на ссылку сведения по устранению неполадок может быть на портале Azure или Microsoft doc.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5653801fb3e4575e642c012721b667f51e791cc1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430870"
---
# <a name="devicemanagementtroubleshootingerrorresource-resource-type"></a>Тип ресурса deviceManagementTroubleshootingErrorResource

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект, представляющий ссылку на ссылку сведения по устранению неполадок может быть на портале Azure или Microsoft doc.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|text|String|Н/Д|
|ссылка|String|Ссылка на веб-ресурс. Может содержать любые из следующих форматирования данных: {{имени участника-пользователя}}, {{DeviceGUID}}, {{UserGUID}}|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorResource",
  "text": "String",
  "link": "String"
}
```





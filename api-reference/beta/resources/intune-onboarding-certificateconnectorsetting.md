---
title: Тип ресурса certificateConnectorSetting
description: Параметры соединителя сертификата.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5886418aaddede43f2397ad626028598a63a0066
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398655"
---
# <a name="certificateconnectorsetting-resource-type"></a>Тип ресурса certificateConnectorSetting

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры соединителя сертификата.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|status|Int32|Состояние соединителя сертификата|
|certExpiryTime|DateTimeOffset|Срок действия сертификата времени|
|enrollmentError|String|Ошибка регистрации сертификата соединителя|
|lastConnectorConnectionTime|DateTimeOffset|Время последнего сертификата подключенных соединителя|
|connectorVersion|String|Версия сертификата соединителя|
|lastUploadVersion|Int64|Версия последнего загруженного сертификата соединителя|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.certificateConnectorSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.certificateConnectorSetting",
  "status": 1024,
  "certExpiryTime": "String (timestamp)",
  "enrollmentError": "String",
  "lastConnectorConnectionTime": "String (timestamp)",
  "connectorVersion": "String",
  "lastUploadVersion": 1024
}
```





---
title: тип ресурса certificateConnectorSetting
description: Параметры соединитетеля сертификата.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0c1c99e202c83dce63e78ba97fc8ad9e27653729
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788922"
---
# <a name="certificateconnectorsetting-resource-type"></a>тип ресурса certificateConnectorSetting

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры соединитетеля сертификата.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|status|Int32|Состояние соединиттеля сертификата|
|certExpiryTime|DateTimeOffset|Срок действия сертификата|
|enrollmentError|Строка|Ошибка регистрации соединители сертификата|
|lastConnectorConnectionTime|DateTimeOffset|Последний раз подключение соединиттеля сертификата|
|connectorVersion|Строка|Версия соединиттеля сертификата|
|lastUploadVersion|Int64|Версия последнего загруженного соединиттеля сертификата|

## <a name="relationships"></a>Связи
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




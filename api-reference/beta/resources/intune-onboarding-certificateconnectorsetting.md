---
title: тип ресурса certificateConnectorSetting
description: Параметры соединитетеля сертификата.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e8df09583947c35eb62255d4f743c150daf73f59
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017249"
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
|enrollmentError|String|Ошибка регистрации соединители сертификата|
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




---
title: тип ресурса certificateConnectorSetting
description: Параметры соединитетеля сертификата.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 31b8ec7fcfe95e459e6454635b7b5e0a37c16cdec45eba5515a24165ad5ad80d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54206251"
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





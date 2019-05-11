---
title: Тип ресурса Цертификатеконнекторсеттинг
description: Параметры соединителя сертификатов.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4a980e6bf8dd97141fc3fc5a078beedbd0348a79
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940465"
---
# <a name="certificateconnectorsetting-resource-type"></a>Тип ресурса Цертификатеконнекторсеттинг

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры соединителя сертификатов.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|status|Int32|Состояние соединителя сертификатов|
|Цертекспиритиме|DateTimeOffset|Время истечения срока действия сертификата|
|Енроллментеррор|Строка|Ошибка регистрации соединителя сертификатов|
|Ластконнекторконнектионтиме|DateTimeOffset|Время последнего подключения к соединителю сертификата|
|Коннекторверсион|Строка|Версия соединителя сертификатов|
|Ластуплоадверсион|Int64|Версия последнего отправленного соединителя сертификатов|

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





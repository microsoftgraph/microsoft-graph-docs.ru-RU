---
title: Тип ресурса Цертификатеконнекторсеттинг
description: Параметры соединителя сертификатов.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 09f4baf9ddd8be630c432fcec5d7df71c442bbe2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168308"
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
|Енроллментеррор|String|Ошибка регистрации соединителя сертификатов|
|Ластконнекторконнектионтиме|DateTimeOffset|Время последнего подключения к соединителю сертификата|
|Коннекторверсион|String|Версия соединителя сертификатов|
|Ластуплоадверсион|Int64|Версия последнего отправленного соединителя сертификатов|

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





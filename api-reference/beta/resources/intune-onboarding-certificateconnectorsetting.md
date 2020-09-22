---
title: Тип ресурса Цертификатеконнекторсеттинг
description: Параметры соединителя сертификатов.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 29585af2586a849c5c75bbf04878d3aadcd8d710
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029794"
---
# <a name="certificateconnectorsetting-resource-type"></a>Тип ресурса Цертификатеконнекторсеттинг

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры соединителя сертификатов.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|status|Int32|Состояние соединителя сертификатов|
|цертекспиритиме|DateTimeOffset|Время истечения срока действия сертификата|
|енроллментеррор|String|Ошибка регистрации соединителя сертификатов|
|ластконнекторконнектионтиме|DateTimeOffset|Время последнего подключения к соединителю сертификата|
|коннекторверсион|String|Версия соединителя сертификатов|
|ластуплоадверсион|Int64|Версия последнего отправленного соединителя сертификатов|

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







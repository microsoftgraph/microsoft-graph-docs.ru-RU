---
title: Тип ресурса Цертификатеконнекторсеттинг
description: Параметры соединителя сертификатов.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 60c7ac990a4eccd1f4faf0fd8f32c42a1e1addba
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36341986"
---
# <a name="certificateconnectorsetting-resource-type"></a>Тип ресурса Цертификатеконнекторсеттинг

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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




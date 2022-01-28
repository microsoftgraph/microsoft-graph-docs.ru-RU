---
title: тип ресурса teamworkOnPremisesCalendarSyncConfiguration
description: Представляет сведения об учетной записи, используемой для синхронизации календарей в Microsoft Teams клиенте устройства с Microsoft Teams включенной поддержкой.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7b5b8d95cc2743b15c6903852a0d81c41949148a
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262590"
---
# <a name="teamworkonpremisescalendarsyncconfiguration-resource-type"></a>тип ресурса teamworkOnPremisesCalendarSyncConfiguration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения об учетной записи, используемой для синхронизации календарей в Microsoft Teams клиенте Microsoft Teams [устройства с](../resources/teamworkdevice.md) включенной поддержкой.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|domain|String|Полное доменное имя (FQDN) Skype для бизнеса Server. Используйте домен Exchange, если Skype для бизнеса SIP отличается от Exchange домена пользователя.|
|domainUserName|String|Например, домен и имя `Seattle\RanierConf`пользователя консоли.|
|smtpAddress|String|Простой адрес протокола передачи почты (SMTP) учетной записи пользователя. Это необходимо только в том случае, если другое имя пользователя (UPN) используется для регистрации Exchange, кроме Microsoft Teams и Skype для бизнеса. Это распространенный сценарий в гибридной среде, где используется Exchange сервер.|


## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkOnPremisesCalendarSyncConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkOnPremisesCalendarSyncConfiguration",
  "domain": "String",
  "domainUserName": "String",
  "smtpAddress": "String"
}
```


---
title: Тип ресурса ИосвпнсекуритяссоЦиатионпараметерс
description: Параметры сопоставления безопасности VPN
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 10ba08470caea556fa6e77c4b3ff912dfeef3990
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356859"
---
# <a name="iosvpnsecurityassociationparameters-resource-type"></a>Тип ресурса ИосвпнсекуритяссоЦиатионпараметерс

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры сопоставления безопасности VPN

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|секуритенкриптионалгорисм|[впненкриптионалгорисмтипе](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|Алгоритм шифрования. Возможные значения: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`.|
|секуритинтегритялгорисм|[впнинтегритялгорисмтипе](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|Алгоритм проверки целостности. Возможные значения: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`.|
|секуритидиффиехеллманграуп|Int32|Группа Диффи Диффи — Хелмана|
|лифетимеинминутес|Int32|Срок действия (в минутах)|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVpnSecurityAssociationParameters",
  "securityEncryptionAlgorithm": "String",
  "securityIntegrityAlgorithm": "String",
  "securityDiffieHellmanGroup": 1024,
  "lifetimeInMinutes": 1024
}
```




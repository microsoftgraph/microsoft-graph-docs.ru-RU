---
title: Тип ресурса ИосвпнсекуритяссоЦиатионпараметерс
description: Параметры сопоставления безопасности VPN
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 85f69b9cf8e19acf09ca0ca179df6cd7fee2fbd9
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793901"
---
# <a name="iosvpnsecurityassociationparameters-resource-type"></a>Тип ресурса ИосвпнсекуритяссоЦиатионпараметерс

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры сопоставления безопасности VPN

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|секуритенкриптионалгорисм|[vpnEncryptionAlgorithmType](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|Алгоритм шифрования. Возможные значения: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.|
|секуритинтегритялгорисм|[vpnIntegrityAlgorithmType](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|Алгоритм проверки целостности. Возможные значения: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.|
|секуритидиффиехеллманграуп|Int32|Группа Диффи Диффи — Хелмана|
|лифетимеинминутес|Int32|Срок действия (в минутах)|

## <a name="relationships"></a>Связи
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




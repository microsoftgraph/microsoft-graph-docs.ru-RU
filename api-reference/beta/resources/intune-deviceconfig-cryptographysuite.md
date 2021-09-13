---
title: тип ресурса cryptographySuite
description: Параметры ассоциации безопасности VPN
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de14441335242a8a59f4011055ebae1f5cedc6e2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59127382"
---
# <a name="cryptographysuite-resource-type"></a>тип ресурса cryptographySuite

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры ассоциации безопасности VPN

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|encryptionMethod|[vpnEncryptionAlgorithmType](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|Метод шифрования. Возможные значения: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`, `chaCha20Poly1305`.|
|integrityCheckMethod|[vpnIntegrityAlgorithmType](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|Метод проверки целостности. Возможные значения: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.|
|dhGroup|[diffieHellmanGroup](../resources/intune-deviceconfig-diffiehellmangroup.md)|Diffie Hellman Group. Возможные значения: `group1`, `group2`, `group14`, `ecp256`, `ecp384`, `group24`.|
|cipherTransformConstants|[vpnEncryptionAlgorithmType](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|Константы преобразования шифров. Возможные значения: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`, `chaCha20Poly1305`.|
|проверка подлинностиTransformConstants|[authenticationTransformConstant](../resources/intune-deviceconfig-authenticationtransformconstant.md)|Преобразование констант проверки подлинности. Возможные значения: `md5_96`, `sha1_96`, `sha_256_128`, `aes128Gcm`, `aes192Gcm`, `aes256Gcm`.|
|pfsGroup|[perfectForwardSecrecyGroup](../resources/intune-deviceconfig-perfectforwardsecrecygroup.md)|Perfect Forward Secrecy Group. Возможные значения: `pfs1`, `pfs2`, `pfs2048`, `ecp256`, `ecp384`, `pfsMM`, `pfs24`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cryptographySuite"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cryptographySuite",
  "encryptionMethod": "String",
  "integrityCheckMethod": "String",
  "dhGroup": "String",
  "cipherTransformConstants": "String",
  "authenticationTransformConstants": "String",
  "pfsGroup": "String"
}
```




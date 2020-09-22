---
title: Тип ресурса Криптографисуите
description: Параметры сопоставления безопасности VPN
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 686799364201b004470aa80ebe1df5a1eac98fe7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998798"
---
# <a name="cryptographysuite-resource-type"></a><span data-ttu-id="561b1-103">Тип ресурса Криптографисуите</span><span class="sxs-lookup"><span data-stu-id="561b1-103">cryptographySuite resource type</span></span>

<span data-ttu-id="561b1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="561b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="561b1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="561b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="561b1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="561b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="561b1-107">Параметры сопоставления безопасности VPN</span><span class="sxs-lookup"><span data-stu-id="561b1-107">VPN Security Association Parameters</span></span>

## <a name="properties"></a><span data-ttu-id="561b1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="561b1-108">Properties</span></span>
|<span data-ttu-id="561b1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="561b1-109">Property</span></span>|<span data-ttu-id="561b1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="561b1-110">Type</span></span>|<span data-ttu-id="561b1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="561b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="561b1-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="561b1-112">encryptionMethod</span></span>|[<span data-ttu-id="561b1-113">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="561b1-113">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="561b1-114">Метод шифрования.</span><span class="sxs-lookup"><span data-stu-id="561b1-114">Encryption Method.</span></span> <span data-ttu-id="561b1-115">Возможные значения: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span><span class="sxs-lookup"><span data-stu-id="561b1-115">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span></span>|
|<span data-ttu-id="561b1-116">интегритичеккмесод</span><span class="sxs-lookup"><span data-stu-id="561b1-116">integrityCheckMethod</span></span>|[<span data-ttu-id="561b1-117">vpnIntegrityAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="561b1-117">vpnIntegrityAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|<span data-ttu-id="561b1-118">Метод проверки целостности.</span><span class="sxs-lookup"><span data-stu-id="561b1-118">Integrity Check Method.</span></span> <span data-ttu-id="561b1-119">Возможные значения: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.</span><span class="sxs-lookup"><span data-stu-id="561b1-119">Possible values are: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.</span></span>|
|<span data-ttu-id="561b1-120">дхграуп</span><span class="sxs-lookup"><span data-stu-id="561b1-120">dhGroup</span></span>|[<span data-ttu-id="561b1-121">diffieHellmanGroup</span><span class="sxs-lookup"><span data-stu-id="561b1-121">diffieHellmanGroup</span></span>](../resources/intune-deviceconfig-diffiehellmangroup.md)|<span data-ttu-id="561b1-122">Группа Диффи Диффи/Хелмана.</span><span class="sxs-lookup"><span data-stu-id="561b1-122">Diffie Hellman Group.</span></span> <span data-ttu-id="561b1-123">Возможные значения: `group1`, `group2`, `group14`, `ecp256`, `ecp384`, `group24`.</span><span class="sxs-lookup"><span data-stu-id="561b1-123">Possible values are: `group1`, `group2`, `group14`, `ecp256`, `ecp384`, `group24`.</span></span>|
|<span data-ttu-id="561b1-124">Цифертрансформконстантс</span><span class="sxs-lookup"><span data-stu-id="561b1-124">cipherTransformConstants</span></span>|[<span data-ttu-id="561b1-125">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="561b1-125">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="561b1-126">Константы преобразования шифров.</span><span class="sxs-lookup"><span data-stu-id="561b1-126">Cipher Transform Constants.</span></span> <span data-ttu-id="561b1-127">Возможные значения: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span><span class="sxs-lookup"><span data-stu-id="561b1-127">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span></span>|
|<span data-ttu-id="561b1-128">аусентикатионтрансформконстантс</span><span class="sxs-lookup"><span data-stu-id="561b1-128">authenticationTransformConstants</span></span>|[<span data-ttu-id="561b1-129">authenticationTransformConstant</span><span class="sxs-lookup"><span data-stu-id="561b1-129">authenticationTransformConstant</span></span>](../resources/intune-deviceconfig-authenticationtransformconstant.md)|<span data-ttu-id="561b1-130">Константы преобразования проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="561b1-130">Authentication Transform Constants.</span></span> <span data-ttu-id="561b1-131">Возможные значения: `md5_96`, `sha1_96`, `sha_256_128`, `aes128Gcm`, `aes192Gcm`, `aes256Gcm`.</span><span class="sxs-lookup"><span data-stu-id="561b1-131">Possible values are: `md5_96`, `sha1_96`, `sha_256_128`, `aes128Gcm`, `aes192Gcm`, `aes256Gcm`.</span></span>|
|<span data-ttu-id="561b1-132">пфсграуп</span><span class="sxs-lookup"><span data-stu-id="561b1-132">pfsGroup</span></span>|[<span data-ttu-id="561b1-133">perfectForwardSecrecyGroup</span><span class="sxs-lookup"><span data-stu-id="561b1-133">perfectForwardSecrecyGroup</span></span>](../resources/intune-deviceconfig-perfectforwardsecrecygroup.md)|<span data-ttu-id="561b1-134">Безопасная пересылка группы.</span><span class="sxs-lookup"><span data-stu-id="561b1-134">Perfect Forward Secrecy Group.</span></span> <span data-ttu-id="561b1-135">Возможные значения: `pfs1`, `pfs2`, `pfs2048`, `ecp256`, `ecp384`, `pfsMM`, `pfs24`.</span><span class="sxs-lookup"><span data-stu-id="561b1-135">Possible values are: `pfs1`, `pfs2`, `pfs2048`, `ecp256`, `ecp384`, `pfsMM`, `pfs24`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="561b1-136">Связи</span><span class="sxs-lookup"><span data-stu-id="561b1-136">Relationships</span></span>
<span data-ttu-id="561b1-137">Нет</span><span class="sxs-lookup"><span data-stu-id="561b1-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="561b1-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="561b1-138">JSON Representation</span></span>
<span data-ttu-id="561b1-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="561b1-139">Here is a JSON representation of the resource.</span></span>
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







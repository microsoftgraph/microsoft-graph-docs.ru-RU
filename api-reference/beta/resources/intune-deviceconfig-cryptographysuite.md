---
title: Тип ресурса Криптографисуите
description: Параметры сопоставления безопасности VPN
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8c09525fdc65a64272901a8823fe9a3fffbecb62
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790259"
---
# <a name="cryptographysuite-resource-type"></a><span data-ttu-id="91503-103">Тип ресурса Криптографисуите</span><span class="sxs-lookup"><span data-stu-id="91503-103">cryptographySuite resource type</span></span>

<span data-ttu-id="91503-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91503-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91503-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91503-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91503-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91503-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91503-107">Параметры сопоставления безопасности VPN</span><span class="sxs-lookup"><span data-stu-id="91503-107">VPN Security Association Parameters</span></span>

## <a name="properties"></a><span data-ttu-id="91503-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="91503-108">Properties</span></span>
|<span data-ttu-id="91503-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="91503-109">Property</span></span>|<span data-ttu-id="91503-110">Тип</span><span class="sxs-lookup"><span data-stu-id="91503-110">Type</span></span>|<span data-ttu-id="91503-111">Описание</span><span class="sxs-lookup"><span data-stu-id="91503-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91503-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="91503-112">encryptionMethod</span></span>|[<span data-ttu-id="91503-113">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="91503-113">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="91503-114">Метод шифрования.</span><span class="sxs-lookup"><span data-stu-id="91503-114">Encryption Method.</span></span> <span data-ttu-id="91503-115">Возможные значения: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span><span class="sxs-lookup"><span data-stu-id="91503-115">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span></span>|
|<span data-ttu-id="91503-116">интегритичеккмесод</span><span class="sxs-lookup"><span data-stu-id="91503-116">integrityCheckMethod</span></span>|[<span data-ttu-id="91503-117">vpnIntegrityAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="91503-117">vpnIntegrityAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|<span data-ttu-id="91503-118">Метод проверки целостности.</span><span class="sxs-lookup"><span data-stu-id="91503-118">Integrity Check Method.</span></span> <span data-ttu-id="91503-119">Возможные значения: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.</span><span class="sxs-lookup"><span data-stu-id="91503-119">Possible values are: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.</span></span>|
|<span data-ttu-id="91503-120">дхграуп</span><span class="sxs-lookup"><span data-stu-id="91503-120">dhGroup</span></span>|[<span data-ttu-id="91503-121">диффиехеллманграуп</span><span class="sxs-lookup"><span data-stu-id="91503-121">diffieHellmanGroup</span></span>](../resources/intune-deviceconfig-diffiehellmangroup.md)|<span data-ttu-id="91503-122">Группа Диффи Диффи/Хелмана.</span><span class="sxs-lookup"><span data-stu-id="91503-122">Diffie Hellman Group.</span></span> <span data-ttu-id="91503-123">Возможные значения: `group1`, `group2`, `group14`, `ecp256`, `ecp384`, `group24`.</span><span class="sxs-lookup"><span data-stu-id="91503-123">Possible values are: `group1`, `group2`, `group14`, `ecp256`, `ecp384`, `group24`.</span></span>|
|<span data-ttu-id="91503-124">Цифертрансформконстантс</span><span class="sxs-lookup"><span data-stu-id="91503-124">cipherTransformConstants</span></span>|[<span data-ttu-id="91503-125">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="91503-125">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="91503-126">Константы преобразования шифров.</span><span class="sxs-lookup"><span data-stu-id="91503-126">Cipher Transform Constants.</span></span> <span data-ttu-id="91503-127">Возможные значения: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span><span class="sxs-lookup"><span data-stu-id="91503-127">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span></span>|
|<span data-ttu-id="91503-128">аусентикатионтрансформконстантс</span><span class="sxs-lookup"><span data-stu-id="91503-128">authenticationTransformConstants</span></span>|[<span data-ttu-id="91503-129">аусентикатионтрансформконстант</span><span class="sxs-lookup"><span data-stu-id="91503-129">authenticationTransformConstant</span></span>](../resources/intune-deviceconfig-authenticationtransformconstant.md)|<span data-ttu-id="91503-130">Константы преобразования проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="91503-130">Authentication Transform Constants.</span></span> <span data-ttu-id="91503-131">Возможные значения: `md5_96`, `sha1_96`, `sha_256_128`, `aes128Gcm`, `aes192Gcm`, `aes256Gcm`.</span><span class="sxs-lookup"><span data-stu-id="91503-131">Possible values are: `md5_96`, `sha1_96`, `sha_256_128`, `aes128Gcm`, `aes192Gcm`, `aes256Gcm`.</span></span>|
|<span data-ttu-id="91503-132">пфсграуп</span><span class="sxs-lookup"><span data-stu-id="91503-132">pfsGroup</span></span>|[<span data-ttu-id="91503-133">перфектфорвардсекрециграуп</span><span class="sxs-lookup"><span data-stu-id="91503-133">perfectForwardSecrecyGroup</span></span>](../resources/intune-deviceconfig-perfectforwardsecrecygroup.md)|<span data-ttu-id="91503-134">Безопасная пересылка группы.</span><span class="sxs-lookup"><span data-stu-id="91503-134">Perfect Forward Secrecy Group.</span></span> <span data-ttu-id="91503-135">Возможные значения: `pfs1`, `pfs2`, `pfs2048`, `ecp256`, `ecp384`, `pfsMM`, `pfs24`.</span><span class="sxs-lookup"><span data-stu-id="91503-135">Possible values are: `pfs1`, `pfs2`, `pfs2048`, `ecp256`, `ecp384`, `pfsMM`, `pfs24`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91503-136">Связи</span><span class="sxs-lookup"><span data-stu-id="91503-136">Relationships</span></span>
<span data-ttu-id="91503-137">Нет</span><span class="sxs-lookup"><span data-stu-id="91503-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91503-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91503-138">JSON Representation</span></span>
<span data-ttu-id="91503-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91503-139">Here is a JSON representation of the resource.</span></span>
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




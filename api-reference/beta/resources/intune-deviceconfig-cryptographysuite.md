---
title: Тип ресурса Криптографисуите
description: Параметры сопоставления безопасности VPN
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9e2de92f47203888df2e167ae06e025b1cad0190
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729807"
---
# <a name="cryptographysuite-resource-type"></a><span data-ttu-id="324e5-103">Тип ресурса Криптографисуите</span><span class="sxs-lookup"><span data-stu-id="324e5-103">cryptographySuite resource type</span></span>

<span data-ttu-id="324e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="324e5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="324e5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="324e5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="324e5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="324e5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="324e5-107">Параметры сопоставления безопасности VPN</span><span class="sxs-lookup"><span data-stu-id="324e5-107">VPN Security Association Parameters</span></span>

## <a name="properties"></a><span data-ttu-id="324e5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="324e5-108">Properties</span></span>
|<span data-ttu-id="324e5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="324e5-109">Property</span></span>|<span data-ttu-id="324e5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="324e5-110">Type</span></span>|<span data-ttu-id="324e5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="324e5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="324e5-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="324e5-112">encryptionMethod</span></span>|[<span data-ttu-id="324e5-113">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="324e5-113">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="324e5-114">Метод шифрования.</span><span class="sxs-lookup"><span data-stu-id="324e5-114">Encryption Method.</span></span> <span data-ttu-id="324e5-115">Возможные значения: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span><span class="sxs-lookup"><span data-stu-id="324e5-115">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span></span>|
|<span data-ttu-id="324e5-116">интегритичеккмесод</span><span class="sxs-lookup"><span data-stu-id="324e5-116">integrityCheckMethod</span></span>|[<span data-ttu-id="324e5-117">vpnIntegrityAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="324e5-117">vpnIntegrityAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|<span data-ttu-id="324e5-118">Метод проверки целостности.</span><span class="sxs-lookup"><span data-stu-id="324e5-118">Integrity Check Method.</span></span> <span data-ttu-id="324e5-119">Возможные значения: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.</span><span class="sxs-lookup"><span data-stu-id="324e5-119">Possible values are: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.</span></span>|
|<span data-ttu-id="324e5-120">дхграуп</span><span class="sxs-lookup"><span data-stu-id="324e5-120">dhGroup</span></span>|[<span data-ttu-id="324e5-121">diffieHellmanGroup</span><span class="sxs-lookup"><span data-stu-id="324e5-121">diffieHellmanGroup</span></span>](../resources/intune-deviceconfig-diffiehellmangroup.md)|<span data-ttu-id="324e5-122">Группа Диффи Диффи/Хелмана.</span><span class="sxs-lookup"><span data-stu-id="324e5-122">Diffie Hellman Group.</span></span> <span data-ttu-id="324e5-123">Возможные значения: `group1`, `group2`, `group14`, `ecp256`, `ecp384`, `group24`.</span><span class="sxs-lookup"><span data-stu-id="324e5-123">Possible values are: `group1`, `group2`, `group14`, `ecp256`, `ecp384`, `group24`.</span></span>|
|<span data-ttu-id="324e5-124">Цифертрансформконстантс</span><span class="sxs-lookup"><span data-stu-id="324e5-124">cipherTransformConstants</span></span>|[<span data-ttu-id="324e5-125">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="324e5-125">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="324e5-126">Константы преобразования шифров.</span><span class="sxs-lookup"><span data-stu-id="324e5-126">Cipher Transform Constants.</span></span> <span data-ttu-id="324e5-127">Возможные значения: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span><span class="sxs-lookup"><span data-stu-id="324e5-127">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span></span>|
|<span data-ttu-id="324e5-128">аусентикатионтрансформконстантс</span><span class="sxs-lookup"><span data-stu-id="324e5-128">authenticationTransformConstants</span></span>|[<span data-ttu-id="324e5-129">authenticationTransformConstant</span><span class="sxs-lookup"><span data-stu-id="324e5-129">authenticationTransformConstant</span></span>](../resources/intune-deviceconfig-authenticationtransformconstant.md)|<span data-ttu-id="324e5-130">Константы преобразования проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="324e5-130">Authentication Transform Constants.</span></span> <span data-ttu-id="324e5-131">Возможные значения: `md5_96`, `sha1_96`, `sha_256_128`, `aes128Gcm`, `aes192Gcm`, `aes256Gcm`.</span><span class="sxs-lookup"><span data-stu-id="324e5-131">Possible values are: `md5_96`, `sha1_96`, `sha_256_128`, `aes128Gcm`, `aes192Gcm`, `aes256Gcm`.</span></span>|
|<span data-ttu-id="324e5-132">пфсграуп</span><span class="sxs-lookup"><span data-stu-id="324e5-132">pfsGroup</span></span>|[<span data-ttu-id="324e5-133">perfectForwardSecrecyGroup</span><span class="sxs-lookup"><span data-stu-id="324e5-133">perfectForwardSecrecyGroup</span></span>](../resources/intune-deviceconfig-perfectforwardsecrecygroup.md)|<span data-ttu-id="324e5-134">Безопасная пересылка группы.</span><span class="sxs-lookup"><span data-stu-id="324e5-134">Perfect Forward Secrecy Group.</span></span> <span data-ttu-id="324e5-135">Возможные значения: `pfs1`, `pfs2`, `pfs2048`, `ecp256`, `ecp384`, `pfsMM`, `pfs24`.</span><span class="sxs-lookup"><span data-stu-id="324e5-135">Possible values are: `pfs1`, `pfs2`, `pfs2048`, `ecp256`, `ecp384`, `pfsMM`, `pfs24`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="324e5-136">Связи</span><span class="sxs-lookup"><span data-stu-id="324e5-136">Relationships</span></span>
<span data-ttu-id="324e5-137">Нет</span><span class="sxs-lookup"><span data-stu-id="324e5-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="324e5-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="324e5-138">JSON Representation</span></span>
<span data-ttu-id="324e5-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="324e5-139">Here is a JSON representation of the resource.</span></span>
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






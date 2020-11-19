---
title: Тип ресурса Криптографисуите
description: Параметры сопоставления безопасности VPN
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 26784db84c461566fa8e2d5c9d6b649fc4bfc9b8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256815"
---
# <a name="cryptographysuite-resource-type"></a><span data-ttu-id="d89ad-103">Тип ресурса Криптографисуите</span><span class="sxs-lookup"><span data-stu-id="d89ad-103">cryptographySuite resource type</span></span>

<span data-ttu-id="d89ad-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d89ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d89ad-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d89ad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d89ad-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d89ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d89ad-107">Параметры сопоставления безопасности VPN</span><span class="sxs-lookup"><span data-stu-id="d89ad-107">VPN Security Association Parameters</span></span>

## <a name="properties"></a><span data-ttu-id="d89ad-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d89ad-108">Properties</span></span>
|<span data-ttu-id="d89ad-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d89ad-109">Property</span></span>|<span data-ttu-id="d89ad-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d89ad-110">Type</span></span>|<span data-ttu-id="d89ad-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d89ad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d89ad-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="d89ad-112">encryptionMethod</span></span>|[<span data-ttu-id="d89ad-113">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="d89ad-113">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="d89ad-114">Метод шифрования.</span><span class="sxs-lookup"><span data-stu-id="d89ad-114">Encryption Method.</span></span> <span data-ttu-id="d89ad-115">Возможные значения: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span><span class="sxs-lookup"><span data-stu-id="d89ad-115">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span></span>|
|<span data-ttu-id="d89ad-116">интегритичеккмесод</span><span class="sxs-lookup"><span data-stu-id="d89ad-116">integrityCheckMethod</span></span>|[<span data-ttu-id="d89ad-117">vpnIntegrityAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="d89ad-117">vpnIntegrityAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|<span data-ttu-id="d89ad-118">Метод проверки целостности.</span><span class="sxs-lookup"><span data-stu-id="d89ad-118">Integrity Check Method.</span></span> <span data-ttu-id="d89ad-119">Возможные значения: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.</span><span class="sxs-lookup"><span data-stu-id="d89ad-119">Possible values are: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.</span></span>|
|<span data-ttu-id="d89ad-120">дхграуп</span><span class="sxs-lookup"><span data-stu-id="d89ad-120">dhGroup</span></span>|[<span data-ttu-id="d89ad-121">diffieHellmanGroup</span><span class="sxs-lookup"><span data-stu-id="d89ad-121">diffieHellmanGroup</span></span>](../resources/intune-deviceconfig-diffiehellmangroup.md)|<span data-ttu-id="d89ad-122">Группа Диффи Диффи/Хелмана.</span><span class="sxs-lookup"><span data-stu-id="d89ad-122">Diffie Hellman Group.</span></span> <span data-ttu-id="d89ad-123">Возможные значения: `group1`, `group2`, `group14`, `ecp256`, `ecp384`, `group24`.</span><span class="sxs-lookup"><span data-stu-id="d89ad-123">Possible values are: `group1`, `group2`, `group14`, `ecp256`, `ecp384`, `group24`.</span></span>|
|<span data-ttu-id="d89ad-124">Цифертрансформконстантс</span><span class="sxs-lookup"><span data-stu-id="d89ad-124">cipherTransformConstants</span></span>|[<span data-ttu-id="d89ad-125">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="d89ad-125">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="d89ad-126">Константы преобразования шифров.</span><span class="sxs-lookup"><span data-stu-id="d89ad-126">Cipher Transform Constants.</span></span> <span data-ttu-id="d89ad-127">Возможные значения: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span><span class="sxs-lookup"><span data-stu-id="d89ad-127">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span></span>|
|<span data-ttu-id="d89ad-128">аусентикатионтрансформконстантс</span><span class="sxs-lookup"><span data-stu-id="d89ad-128">authenticationTransformConstants</span></span>|[<span data-ttu-id="d89ad-129">authenticationTransformConstant</span><span class="sxs-lookup"><span data-stu-id="d89ad-129">authenticationTransformConstant</span></span>](../resources/intune-deviceconfig-authenticationtransformconstant.md)|<span data-ttu-id="d89ad-130">Константы преобразования проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="d89ad-130">Authentication Transform Constants.</span></span> <span data-ttu-id="d89ad-131">Возможные значения: `md5_96`, `sha1_96`, `sha_256_128`, `aes128Gcm`, `aes192Gcm`, `aes256Gcm`.</span><span class="sxs-lookup"><span data-stu-id="d89ad-131">Possible values are: `md5_96`, `sha1_96`, `sha_256_128`, `aes128Gcm`, `aes192Gcm`, `aes256Gcm`.</span></span>|
|<span data-ttu-id="d89ad-132">пфсграуп</span><span class="sxs-lookup"><span data-stu-id="d89ad-132">pfsGroup</span></span>|[<span data-ttu-id="d89ad-133">perfectForwardSecrecyGroup</span><span class="sxs-lookup"><span data-stu-id="d89ad-133">perfectForwardSecrecyGroup</span></span>](../resources/intune-deviceconfig-perfectforwardsecrecygroup.md)|<span data-ttu-id="d89ad-134">Безопасная пересылка группы.</span><span class="sxs-lookup"><span data-stu-id="d89ad-134">Perfect Forward Secrecy Group.</span></span> <span data-ttu-id="d89ad-135">Возможные значения: `pfs1`, `pfs2`, `pfs2048`, `ecp256`, `ecp384`, `pfsMM`, `pfs24`.</span><span class="sxs-lookup"><span data-stu-id="d89ad-135">Possible values are: `pfs1`, `pfs2`, `pfs2048`, `ecp256`, `ecp384`, `pfsMM`, `pfs24`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d89ad-136">Связи</span><span class="sxs-lookup"><span data-stu-id="d89ad-136">Relationships</span></span>
<span data-ttu-id="d89ad-137">Нет</span><span class="sxs-lookup"><span data-stu-id="d89ad-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d89ad-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d89ad-138">JSON Representation</span></span>
<span data-ttu-id="d89ad-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d89ad-139">Here is a JSON representation of the resource.</span></span>
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





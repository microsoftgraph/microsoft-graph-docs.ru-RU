---
title: Тип ресурса ИосвпнсекуритяссоЦиатионпараметерс
description: Параметры сопоставления безопасности VPN
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d3da905a68222b60bef7225f34afc2b4a0b39a50
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790498"
---
# <a name="iosvpnsecurityassociationparameters-resource-type"></a><span data-ttu-id="6e550-103">Тип ресурса ИосвпнсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="6e550-103">iosVpnSecurityAssociationParameters resource type</span></span>

> <span data-ttu-id="6e550-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e550-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e550-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e550-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e550-106">Параметры сопоставления безопасности VPN</span><span class="sxs-lookup"><span data-stu-id="6e550-106">VPN Security Association Parameters</span></span>

## <a name="properties"></a><span data-ttu-id="6e550-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e550-107">Properties</span></span>
|<span data-ttu-id="6e550-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e550-108">Property</span></span>|<span data-ttu-id="6e550-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6e550-109">Type</span></span>|<span data-ttu-id="6e550-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6e550-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e550-111">секуритенкриптионалгорисм</span><span class="sxs-lookup"><span data-stu-id="6e550-111">securityEncryptionAlgorithm</span></span>|[<span data-ttu-id="6e550-112">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="6e550-112">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="6e550-113">Алгоритм шифрования.</span><span class="sxs-lookup"><span data-stu-id="6e550-113">Encryption algorithm.</span></span> <span data-ttu-id="6e550-114">Возможные значения: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`.</span><span class="sxs-lookup"><span data-stu-id="6e550-114">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`.</span></span>|
|<span data-ttu-id="6e550-115">секуритинтегритялгорисм</span><span class="sxs-lookup"><span data-stu-id="6e550-115">securityIntegrityAlgorithm</span></span>|[<span data-ttu-id="6e550-116">vpnIntegrityAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="6e550-116">vpnIntegrityAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|<span data-ttu-id="6e550-117">Алгоритм проверки целостности.</span><span class="sxs-lookup"><span data-stu-id="6e550-117">Integrity algorithm.</span></span> <span data-ttu-id="6e550-118">Возможные значения: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`.</span><span class="sxs-lookup"><span data-stu-id="6e550-118">Possible values are: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`.</span></span>|
|<span data-ttu-id="6e550-119">секуритидиффиехеллманграуп</span><span class="sxs-lookup"><span data-stu-id="6e550-119">securityDiffieHellmanGroup</span></span>|<span data-ttu-id="6e550-120">Int32</span><span class="sxs-lookup"><span data-stu-id="6e550-120">Int32</span></span>|<span data-ttu-id="6e550-121">Группа Диффи Диффи — Хелмана</span><span class="sxs-lookup"><span data-stu-id="6e550-121">Diffie-Hellman Group</span></span>|
|<span data-ttu-id="6e550-122">лифетимеинминутес</span><span class="sxs-lookup"><span data-stu-id="6e550-122">lifetimeInMinutes</span></span>|<span data-ttu-id="6e550-123">Int32</span><span class="sxs-lookup"><span data-stu-id="6e550-123">Int32</span></span>|<span data-ttu-id="6e550-124">Срок действия (в минутах)</span><span class="sxs-lookup"><span data-stu-id="6e550-124">Lifetime (minutes)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e550-125">Связи</span><span class="sxs-lookup"><span data-stu-id="6e550-125">Relationships</span></span>
<span data-ttu-id="6e550-126">Нет</span><span class="sxs-lookup"><span data-stu-id="6e550-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e550-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e550-127">JSON Representation</span></span>
<span data-ttu-id="6e550-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e550-128">Here is a JSON representation of the resource.</span></span>
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




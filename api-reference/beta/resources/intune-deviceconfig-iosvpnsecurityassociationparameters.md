---
title: Тип ресурса ИосвпнсекуритяссоЦиатионпараметерс
description: Параметры сопоставления безопасности VPN
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cd53bec653f072dd22554be4e4255997657ab833
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526285"
---
# <a name="iosvpnsecurityassociationparameters-resource-type"></a><span data-ttu-id="ac5eb-103">Тип ресурса ИосвпнсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="ac5eb-103">iosVpnSecurityAssociationParameters resource type</span></span>

<span data-ttu-id="ac5eb-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ac5eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ac5eb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac5eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac5eb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ac5eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac5eb-107">Параметры сопоставления безопасности VPN</span><span class="sxs-lookup"><span data-stu-id="ac5eb-107">VPN Security Association Parameters</span></span>

## <a name="properties"></a><span data-ttu-id="ac5eb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac5eb-108">Properties</span></span>
|<span data-ttu-id="ac5eb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac5eb-109">Property</span></span>|<span data-ttu-id="ac5eb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ac5eb-110">Type</span></span>|<span data-ttu-id="ac5eb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ac5eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac5eb-112">секуритенкриптионалгорисм</span><span class="sxs-lookup"><span data-stu-id="ac5eb-112">securityEncryptionAlgorithm</span></span>|[<span data-ttu-id="ac5eb-113">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="ac5eb-113">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="ac5eb-114">Алгоритм шифрования.</span><span class="sxs-lookup"><span data-stu-id="ac5eb-114">Encryption algorithm.</span></span> <span data-ttu-id="ac5eb-115">Возможные значения: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`.</span><span class="sxs-lookup"><span data-stu-id="ac5eb-115">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`.</span></span>|
|<span data-ttu-id="ac5eb-116">секуритинтегритялгорисм</span><span class="sxs-lookup"><span data-stu-id="ac5eb-116">securityIntegrityAlgorithm</span></span>|[<span data-ttu-id="ac5eb-117">vpnIntegrityAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="ac5eb-117">vpnIntegrityAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|<span data-ttu-id="ac5eb-118">Алгоритм проверки целостности.</span><span class="sxs-lookup"><span data-stu-id="ac5eb-118">Integrity algorithm.</span></span> <span data-ttu-id="ac5eb-119">Возможные значения: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`.</span><span class="sxs-lookup"><span data-stu-id="ac5eb-119">Possible values are: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`.</span></span>|
|<span data-ttu-id="ac5eb-120">секуритидиффиехеллманграуп</span><span class="sxs-lookup"><span data-stu-id="ac5eb-120">securityDiffieHellmanGroup</span></span>|<span data-ttu-id="ac5eb-121">Int32</span><span class="sxs-lookup"><span data-stu-id="ac5eb-121">Int32</span></span>|<span data-ttu-id="ac5eb-122">Группа Диффи Диффи — Хелмана</span><span class="sxs-lookup"><span data-stu-id="ac5eb-122">Diffie-Hellman Group</span></span>|
|<span data-ttu-id="ac5eb-123">лифетимеинминутес</span><span class="sxs-lookup"><span data-stu-id="ac5eb-123">lifetimeInMinutes</span></span>|<span data-ttu-id="ac5eb-124">Int32</span><span class="sxs-lookup"><span data-stu-id="ac5eb-124">Int32</span></span>|<span data-ttu-id="ac5eb-125">Срок действия (в минутах)</span><span class="sxs-lookup"><span data-stu-id="ac5eb-125">Lifetime (minutes)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac5eb-126">Связи</span><span class="sxs-lookup"><span data-stu-id="ac5eb-126">Relationships</span></span>
<span data-ttu-id="ac5eb-127">Нет</span><span class="sxs-lookup"><span data-stu-id="ac5eb-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac5eb-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ac5eb-128">JSON Representation</span></span>
<span data-ttu-id="ac5eb-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac5eb-129">Here is a JSON representation of the resource.</span></span>
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




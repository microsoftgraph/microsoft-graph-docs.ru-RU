---
title: Тип ресурса ИосвпнсекуритяссоЦиатионпараметерс
description: Параметры сопоставления безопасности VPN
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ecf2597222a578d342f69c16c665c493b8c3329
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002730"
---
# <a name="iosvpnsecurityassociationparameters-resource-type"></a><span data-ttu-id="6ba30-103">Тип ресурса ИосвпнсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="6ba30-103">iosVpnSecurityAssociationParameters resource type</span></span>

> <span data-ttu-id="6ba30-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ba30-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ba30-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ba30-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ba30-106">Параметры сопоставления безопасности VPN</span><span class="sxs-lookup"><span data-stu-id="6ba30-106">VPN Security Association Parameters</span></span>

## <a name="properties"></a><span data-ttu-id="6ba30-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ba30-107">Properties</span></span>
|<span data-ttu-id="6ba30-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ba30-108">Property</span></span>|<span data-ttu-id="6ba30-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6ba30-109">Type</span></span>|<span data-ttu-id="6ba30-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6ba30-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ba30-111">Секуритенкриптионалгорисм</span><span class="sxs-lookup"><span data-stu-id="6ba30-111">securityEncryptionAlgorithm</span></span>|[<span data-ttu-id="6ba30-112">Впненкриптионалгорисмтипе</span><span class="sxs-lookup"><span data-stu-id="6ba30-112">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="6ba30-113">Алгоритм шифрования.</span><span class="sxs-lookup"><span data-stu-id="6ba30-113">Encryption algorithm.</span></span> <span data-ttu-id="6ba30-114">Возможные значения: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`.</span><span class="sxs-lookup"><span data-stu-id="6ba30-114">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`.</span></span>|
|<span data-ttu-id="6ba30-115">Секуритинтегритялгорисм</span><span class="sxs-lookup"><span data-stu-id="6ba30-115">securityIntegrityAlgorithm</span></span>|[<span data-ttu-id="6ba30-116">Впнинтегритялгорисмтипе</span><span class="sxs-lookup"><span data-stu-id="6ba30-116">vpnIntegrityAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|<span data-ttu-id="6ba30-117">Алгоритм проверки целостности.</span><span class="sxs-lookup"><span data-stu-id="6ba30-117">Integrity algorithm.</span></span> <span data-ttu-id="6ba30-118">Возможные значения: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`.</span><span class="sxs-lookup"><span data-stu-id="6ba30-118">Possible values are: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`.</span></span>|
|<span data-ttu-id="6ba30-119">Секуритидиффиехеллманграуп</span><span class="sxs-lookup"><span data-stu-id="6ba30-119">securityDiffieHellmanGroup</span></span>|<span data-ttu-id="6ba30-120">Int32</span><span class="sxs-lookup"><span data-stu-id="6ba30-120">Int32</span></span>|<span data-ttu-id="6ba30-121">Группа Диффи Диффи — Хелмана</span><span class="sxs-lookup"><span data-stu-id="6ba30-121">Diffie-Hellman Group</span></span>|
|<span data-ttu-id="6ba30-122">Лифетимеинминутес</span><span class="sxs-lookup"><span data-stu-id="6ba30-122">lifetimeInMinutes</span></span>|<span data-ttu-id="6ba30-123">Int32</span><span class="sxs-lookup"><span data-stu-id="6ba30-123">Int32</span></span>|<span data-ttu-id="6ba30-124">Срок действия (в минутах)</span><span class="sxs-lookup"><span data-stu-id="6ba30-124">Lifetime (minutes)</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ba30-125">Отношения</span><span class="sxs-lookup"><span data-stu-id="6ba30-125">Relationships</span></span>
<span data-ttu-id="6ba30-126">Нет</span><span class="sxs-lookup"><span data-stu-id="6ba30-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ba30-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6ba30-127">JSON Representation</span></span>
<span data-ttu-id="6ba30-128">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ba30-128">Here is a JSON representation of the resource.</span></span>
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






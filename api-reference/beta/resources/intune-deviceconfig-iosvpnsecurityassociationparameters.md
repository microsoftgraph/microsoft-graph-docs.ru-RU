---
title: Тип ресурса ИосвпнсекуритяссоЦиатионпараметерс
description: Параметры сопоставления безопасности VPN
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ce1d257c81f539da9b9b524876560e1516fdb6e1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302952"
---
# <a name="iosvpnsecurityassociationparameters-resource-type"></a><span data-ttu-id="144c3-103">Тип ресурса ИосвпнсекуритяссоЦиатионпараметерс</span><span class="sxs-lookup"><span data-stu-id="144c3-103">iosVpnSecurityAssociationParameters resource type</span></span>

<span data-ttu-id="144c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="144c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="144c3-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="144c3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="144c3-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="144c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="144c3-107">Параметры сопоставления безопасности VPN</span><span class="sxs-lookup"><span data-stu-id="144c3-107">VPN Security Association Parameters</span></span>

## <a name="properties"></a><span data-ttu-id="144c3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="144c3-108">Properties</span></span>
|<span data-ttu-id="144c3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="144c3-109">Property</span></span>|<span data-ttu-id="144c3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="144c3-110">Type</span></span>|<span data-ttu-id="144c3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="144c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="144c3-112">секуритенкриптионалгорисм</span><span class="sxs-lookup"><span data-stu-id="144c3-112">securityEncryptionAlgorithm</span></span>|[<span data-ttu-id="144c3-113">vpnEncryptionAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="144c3-113">vpnEncryptionAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnencryptionalgorithmtype.md)|<span data-ttu-id="144c3-114">Алгоритм шифрования.</span><span class="sxs-lookup"><span data-stu-id="144c3-114">Encryption algorithm.</span></span> <span data-ttu-id="144c3-115">Возможные значения: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span><span class="sxs-lookup"><span data-stu-id="144c3-115">Possible values are: `aes256`, `des`, `tripleDes`, `aes128`, `aes128Gcm`, `aes256Gcm`, `aes192`, `aes192Gcm`.</span></span>|
|<span data-ttu-id="144c3-116">секуритинтегритялгорисм</span><span class="sxs-lookup"><span data-stu-id="144c3-116">securityIntegrityAlgorithm</span></span>|[<span data-ttu-id="144c3-117">vpnIntegrityAlgorithmType</span><span class="sxs-lookup"><span data-stu-id="144c3-117">vpnIntegrityAlgorithmType</span></span>](../resources/intune-deviceconfig-vpnintegrityalgorithmtype.md)|<span data-ttu-id="144c3-118">Алгоритм проверки целостности.</span><span class="sxs-lookup"><span data-stu-id="144c3-118">Integrity algorithm.</span></span> <span data-ttu-id="144c3-119">Возможные значения: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.</span><span class="sxs-lookup"><span data-stu-id="144c3-119">Possible values are: `sha2_256`, `sha1_96`, `sha1_160`, `sha2_384`, `sha2_512`, `md5`.</span></span>|
|<span data-ttu-id="144c3-120">секуритидиффиехеллманграуп</span><span class="sxs-lookup"><span data-stu-id="144c3-120">securityDiffieHellmanGroup</span></span>|<span data-ttu-id="144c3-121">Int32</span><span class="sxs-lookup"><span data-stu-id="144c3-121">Int32</span></span>|<span data-ttu-id="144c3-122">Группа Diffie-Hellman</span><span class="sxs-lookup"><span data-stu-id="144c3-122">Diffie-Hellman Group</span></span>|
|<span data-ttu-id="144c3-123">лифетимеинминутес</span><span class="sxs-lookup"><span data-stu-id="144c3-123">lifetimeInMinutes</span></span>|<span data-ttu-id="144c3-124">Int32</span><span class="sxs-lookup"><span data-stu-id="144c3-124">Int32</span></span>|<span data-ttu-id="144c3-125">Срок действия (в минутах)</span><span class="sxs-lookup"><span data-stu-id="144c3-125">Lifetime (minutes)</span></span>|

## <a name="relationships"></a><span data-ttu-id="144c3-126">Связи</span><span class="sxs-lookup"><span data-stu-id="144c3-126">Relationships</span></span>
<span data-ttu-id="144c3-127">Нет</span><span class="sxs-lookup"><span data-stu-id="144c3-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="144c3-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="144c3-128">JSON Representation</span></span>
<span data-ttu-id="144c3-129">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="144c3-129">Here is a JSON representation of the resource.</span></span>
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





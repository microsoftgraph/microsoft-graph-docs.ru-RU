---
title: тип ресурса updatableAssetError
description: Абстрактный тип, представляюющий ошибку, которая не позволяет службе развертывания зачислить azureADDevice в управление обновлениями или развернуть контент на устройстве
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 4d4375be68aea6dd4cb27c7ae8b78aaf86a2edf1
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067499"
---
# <a name="updatableasseterror-resource-type"></a><span data-ttu-id="58b49-103">тип ресурса updatableAssetError</span><span class="sxs-lookup"><span data-stu-id="58b49-103">updatableAssetError resource type</span></span>

<span data-ttu-id="58b49-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="58b49-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58b49-105">Абстрактный тип, представляюющий ошибку, которая не позволяет службе развертывания зачислить [azureADDevice](../resources/windowsupdates-azureaddevice.md) в управление обновлениями или развернуть содержимое на устройстве.</span><span class="sxs-lookup"><span data-stu-id="58b49-105">An abstract type that represents an error which prevents the deployment service from enrolling an [azureADDevice](../resources/windowsupdates-azureaddevice.md) in update management, or deploying content to the device.</span></span> 

<span data-ttu-id="58b49-106">Все updatable ошибки активов имеют производный [тип, azureADDeviceRegistrationError](../resources/windowsupdates-azureaddeviceregistrationerror.md).</span><span class="sxs-lookup"><span data-stu-id="58b49-106">All updatable asset errors are of the derived type, [azureADDeviceRegistrationError](../resources/windowsupdates-azureaddeviceregistrationerror.md).</span></span>


## <a name="properties"></a><span data-ttu-id="58b49-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="58b49-107">Properties</span></span>
<span data-ttu-id="58b49-108">Нет</span><span class="sxs-lookup"><span data-stu-id="58b49-108">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="58b49-109">Связи</span><span class="sxs-lookup"><span data-stu-id="58b49-109">Relationships</span></span>
<span data-ttu-id="58b49-110">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="58b49-110">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="58b49-111">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="58b49-111">JSON representation</span></span>
<span data-ttu-id="58b49-112">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="58b49-112">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.updatableAssetError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updatableAssetError"
}
```


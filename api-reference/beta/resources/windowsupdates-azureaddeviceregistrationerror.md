---
title: тип ресурса azureADDeviceRegistrationError
description: Ошибка в процессе регистрации устройства Azure AD, которая не позволяет службе зачислить устройство в управление обновлениями или развернуть контент на устройстве.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 1d08ab96d5298c70f34acf89e3c6c4605d9df0a1
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068117"
---
# <a name="azureaddeviceregistrationerror-resource-type"></a><span data-ttu-id="82110-103">тип ресурса azureADDeviceRegistrationError</span><span class="sxs-lookup"><span data-stu-id="82110-103">azureADDeviceRegistrationError resource type</span></span>

<span data-ttu-id="82110-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="82110-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82110-105">Ошибка в процессе регистрации устройства [Azure AD,](../resources/windowsupdates-azureaddevice.md) которая не позволяет службе зачислить устройство в управление обновлениями или развернуть контент на устройстве.</span><span class="sxs-lookup"><span data-stu-id="82110-105">An error in the registration process of an [Azure AD device](../resources/windowsupdates-azureaddevice.md) that prevents the service from enrolling the device in update management or deploying content to the device.</span></span>

<span data-ttu-id="82110-106">Наследует [от updatableAssetError](../resources/windowsupdates-updatableasseterror.md).</span><span class="sxs-lookup"><span data-stu-id="82110-106">Inherits from [updatableAssetError](../resources/windowsupdates-updatableasseterror.md).</span></span>

## <a name="properties"></a><span data-ttu-id="82110-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="82110-107">Properties</span></span>
|<span data-ttu-id="82110-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="82110-108">Property</span></span>|<span data-ttu-id="82110-109">Тип</span><span class="sxs-lookup"><span data-stu-id="82110-109">Type</span></span>|<span data-ttu-id="82110-110">Описание</span><span class="sxs-lookup"><span data-stu-id="82110-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82110-111">reason</span><span class="sxs-lookup"><span data-stu-id="82110-111">reason</span></span>|<span data-ttu-id="82110-112">microsoft.graph.windowsUpdates.azureADDeviceRegistrationErrorReason</span><span class="sxs-lookup"><span data-stu-id="82110-112">microsoft.graph.windowsUpdates.azureADDeviceRegistrationErrorReason</span></span>|<span data-ttu-id="82110-113">Причина, по которой регистрация столкнулась с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="82110-113">The reason why the registration encountered an error.</span></span> <span data-ttu-id="82110-114">Возможные значения: `invalidGlobalDeviceId`, `invalidAzureADDeviceId`, `missingTrustType`, `invalidAzureADJoin`.</span><span class="sxs-lookup"><span data-stu-id="82110-114">Possible values are: `invalidGlobalDeviceId`, `invalidAzureADDeviceId`, `missingTrustType`, `invalidAzureADJoin`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82110-115">Связи</span><span class="sxs-lookup"><span data-stu-id="82110-115">Relationships</span></span>
<span data-ttu-id="82110-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="82110-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="82110-117">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="82110-117">JSON representation</span></span>
<span data-ttu-id="82110-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="82110-118">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.azureADDeviceRegistrationError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.azureADDeviceRegistrationError",
  "reason": "String"
}
```


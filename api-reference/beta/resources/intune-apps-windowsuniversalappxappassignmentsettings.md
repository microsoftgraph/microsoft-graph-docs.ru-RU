---
title: Тип ресурса windowsUniversalAppXAppAssignmentSettings
description: Содержит свойства, используемые при назначении мобильное приложение Windows AppX универсальные группы.
ms.openlocfilehash: 9694ab347be6edd1446df8aa7b46fb3652aee589
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078745"
---
# <a name="windowsuniversalappxappassignmentsettings-resource-type"></a><span data-ttu-id="81a91-103">Тип ресурса windowsUniversalAppXAppAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="81a91-103">windowsUniversalAppXAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="81a91-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="81a91-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81a91-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="81a91-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81a91-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="81a91-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81a91-107">Содержит свойства, используемые при назначении мобильное приложение Windows AppX универсальные группы.</span><span class="sxs-lookup"><span data-stu-id="81a91-107">Contains properties used when assigning a Windows Universal AppX mobile app to a group.</span></span>

<span data-ttu-id="81a91-108">Наследуется от [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="81a91-108">Inherits from [mobileAppAssignmentSettings](../resources/intune-apps-mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="81a91-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="81a91-109">Properties</span></span>
|<span data-ttu-id="81a91-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="81a91-110">Property</span></span>|<span data-ttu-id="81a91-111">Тип</span><span class="sxs-lookup"><span data-stu-id="81a91-111">Type</span></span>|<span data-ttu-id="81a91-112">Описание</span><span class="sxs-lookup"><span data-stu-id="81a91-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81a91-113">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="81a91-113">useDeviceContext</span></span>|<span data-ttu-id="81a91-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="81a91-114">Boolean</span></span>|<span data-ttu-id="81a91-115">Следует ли использовать контекст выполнения устройства для мобильного приложения универсальные AppX Windows.</span><span class="sxs-lookup"><span data-stu-id="81a91-115">Whether or not to use device execution context for Windows Universal AppX mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81a91-116">Связи</span><span class="sxs-lookup"><span data-stu-id="81a91-116">Relationships</span></span>
<span data-ttu-id="81a91-117">Нет</span><span class="sxs-lookup"><span data-stu-id="81a91-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="81a91-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81a91-118">JSON Representation</span></span>
<span data-ttu-id="81a91-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81a91-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUniversalAppXAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXAppAssignmentSettings",
  "useDeviceContext": true
}
```






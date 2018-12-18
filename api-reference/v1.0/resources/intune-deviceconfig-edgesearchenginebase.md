---
title: Тип ресурса edgeSearchEngineBase
description: Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для управляемых с помощью системы MDM устройств. Пользователи могут переопределять эту настройку и изменять поисковую систему по умолчанию, если не установлена политика AllowSearchEngineCustomization.
author: tfitzmac
ms.openlocfilehash: ab7b02e9e158dd711347b27b916fc4bb97c1f2af
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301549"
---
# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="4cfb4-104">Тип ресурса edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="4cfb4-104">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="4cfb4-105">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4cfb4-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4cfb4-106">Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="4cfb4-106">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="4cfb4-107">Пользователи могут переопределять эту настройку и изменять поисковую систему по умолчанию, если не установлена политика AllowSearchEngineCustomization.</span><span class="sxs-lookup"><span data-stu-id="4cfb4-107">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>
## <a name="properties"></a><span data-ttu-id="4cfb4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4cfb4-108">Properties</span></span>
|<span data-ttu-id="4cfb4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4cfb4-109">Property</span></span>|<span data-ttu-id="4cfb4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4cfb4-110">Type</span></span>|<span data-ttu-id="4cfb4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4cfb4-111">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="4cfb4-112">Связи</span><span class="sxs-lookup"><span data-stu-id="4cfb4-112">Relationships</span></span>
<span data-ttu-id="4cfb4-113">Нет</span><span class="sxs-lookup"><span data-stu-id="4cfb4-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4cfb4-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4cfb4-114">JSON Representation</span></span>
<span data-ttu-id="4cfb4-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4cfb4-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineBase"
}
```




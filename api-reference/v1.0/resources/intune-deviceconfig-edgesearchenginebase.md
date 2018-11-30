---
title: Тип ресурса edgeSearchEngineBase
description: Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для управляемых с помощью системы MDM устройств. Пользователи могут переопределять эту настройку и изменять поисковую систему по умолчанию, если не установлена политика AllowSearchEngineCustomization.
ms.openlocfilehash: 505816652890cd72c61b91001dbce2061b76fc11
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024885"
---
# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="6bdc3-104">Тип ресурса edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="6bdc3-104">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="6bdc3-105">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6bdc3-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6bdc3-106">Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="6bdc3-106">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="6bdc3-107">Пользователи могут переопределять эту настройку и изменять поисковую систему по умолчанию, если не установлена политика AllowSearchEngineCustomization.</span><span class="sxs-lookup"><span data-stu-id="6bdc3-107">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>
## <a name="properties"></a><span data-ttu-id="6bdc3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6bdc3-108">Properties</span></span>
|<span data-ttu-id="6bdc3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6bdc3-109">Property</span></span>|<span data-ttu-id="6bdc3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6bdc3-110">Type</span></span>|<span data-ttu-id="6bdc3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6bdc3-111">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="6bdc3-112">Связи</span><span class="sxs-lookup"><span data-stu-id="6bdc3-112">Relationships</span></span>
<span data-ttu-id="6bdc3-113">Нет</span><span class="sxs-lookup"><span data-stu-id="6bdc3-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6bdc3-114">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6bdc3-114">JSON Representation</span></span>
<span data-ttu-id="6bdc3-115">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6bdc3-115">Here is a JSON representation of the resource.</span></span>
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




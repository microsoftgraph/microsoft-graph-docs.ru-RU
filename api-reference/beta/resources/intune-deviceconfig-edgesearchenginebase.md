---
title: Тип ресурса edgeSearchEngineBase
description: Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для управляемых с помощью системы MDM устройств. Пользователи могут переопределять эту настройку и изменять поисковую систему по умолчанию, если не установлена политика AllowSearchEngineCustomization.
author: tfitzmac
ms.openlocfilehash: c60dd1786f5a211947c02f1a9f5f048737ba3788
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346503"
---
# <a name="edgesearchenginebase-resource-type"></a><span data-ttu-id="17d6c-104">Тип ресурса edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="17d6c-104">edgeSearchEngineBase resource type</span></span>

> <span data-ttu-id="17d6c-105">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="17d6c-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="17d6c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="17d6c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="17d6c-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="17d6c-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="17d6c-108">Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для управляемых устройств.</span><span class="sxs-lookup"><span data-stu-id="17d6c-108">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="17d6c-109">Пользователи могут переопределять эту настройку и изменять поисковую систему по умолчанию, если не установлена политика AllowSearchEngineCustomization.</span><span class="sxs-lookup"><span data-stu-id="17d6c-109">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>
## <a name="properties"></a><span data-ttu-id="17d6c-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="17d6c-110">Properties</span></span>
|<span data-ttu-id="17d6c-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="17d6c-111">Property</span></span>|<span data-ttu-id="17d6c-112">Тип</span><span class="sxs-lookup"><span data-stu-id="17d6c-112">Type</span></span>|<span data-ttu-id="17d6c-113">Описание</span><span class="sxs-lookup"><span data-stu-id="17d6c-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="17d6c-114">Связи</span><span class="sxs-lookup"><span data-stu-id="17d6c-114">Relationships</span></span>
<span data-ttu-id="17d6c-115">Нет</span><span class="sxs-lookup"><span data-stu-id="17d6c-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="17d6c-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="17d6c-116">JSON Representation</span></span>
<span data-ttu-id="17d6c-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17d6c-117">Here is a JSON representation of the resource.</span></span>
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






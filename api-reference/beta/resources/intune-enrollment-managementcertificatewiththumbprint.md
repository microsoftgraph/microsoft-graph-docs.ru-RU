---
title: Тип ресурса managementCertificateWithThumbprint
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 03846890822cae02a2eb04fc058895992119c98a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348939"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="3fcac-103">Тип ресурса managementCertificateWithThumbprint</span><span class="sxs-lookup"><span data-stu-id="3fcac-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="3fcac-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3fcac-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3fcac-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fcac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3fcac-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3fcac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3fcac-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3fcac-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="3fcac-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3fcac-108">Properties</span></span>
|<span data-ttu-id="3fcac-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3fcac-109">Property</span></span>|<span data-ttu-id="3fcac-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3fcac-110">Type</span></span>|<span data-ttu-id="3fcac-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3fcac-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fcac-112">отпечаток</span><span class="sxs-lookup"><span data-stu-id="3fcac-112">thumbprint</span></span>|<span data-ttu-id="3fcac-113">String.</span><span class="sxs-lookup"><span data-stu-id="3fcac-113">String</span></span>|<span data-ttu-id="3fcac-114">Отпечаток сертификата, управление</span><span class="sxs-lookup"><span data-stu-id="3fcac-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="3fcac-115">certificate</span><span class="sxs-lookup"><span data-stu-id="3fcac-115">certificate</span></span>|<span data-ttu-id="3fcac-116">String</span><span class="sxs-lookup"><span data-stu-id="3fcac-116">String</span></span>|<span data-ttu-id="3fcac-117">Управление сертификат кодировке Base 64</span><span class="sxs-lookup"><span data-stu-id="3fcac-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="3fcac-118">Связи</span><span class="sxs-lookup"><span data-stu-id="3fcac-118">Relationships</span></span>
<span data-ttu-id="3fcac-119">Нет</span><span class="sxs-lookup"><span data-stu-id="3fcac-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3fcac-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3fcac-120">JSON Representation</span></span>
<span data-ttu-id="3fcac-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3fcac-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementCertificateWithThumbprint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCertificateWithThumbprint",
  "thumbprint": "String",
  "certificate": "String"
}
```






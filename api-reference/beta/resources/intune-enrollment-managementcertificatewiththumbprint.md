---
title: Тип ресурса managementCertificateWithThumbprint
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6e6259c1f90547ff875fa31d3f383606749bc0dd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983354"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="c2d3e-103">Тип ресурса managementCertificateWithThumbprint</span><span class="sxs-lookup"><span data-stu-id="c2d3e-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="c2d3e-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c2d3e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2d3e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2d3e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2d3e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c2d3e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2d3e-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c2d3e-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="c2d3e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2d3e-108">Properties</span></span>
|<span data-ttu-id="c2d3e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2d3e-109">Property</span></span>|<span data-ttu-id="c2d3e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c2d3e-110">Type</span></span>|<span data-ttu-id="c2d3e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c2d3e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2d3e-112">отпечаток</span><span class="sxs-lookup"><span data-stu-id="c2d3e-112">thumbprint</span></span>|<span data-ttu-id="c2d3e-113">String</span><span class="sxs-lookup"><span data-stu-id="c2d3e-113">String</span></span>|<span data-ttu-id="c2d3e-114">Отпечаток сертификата, управление</span><span class="sxs-lookup"><span data-stu-id="c2d3e-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="c2d3e-115">certificate</span><span class="sxs-lookup"><span data-stu-id="c2d3e-115">certificate</span></span>|<span data-ttu-id="c2d3e-116">String</span><span class="sxs-lookup"><span data-stu-id="c2d3e-116">String</span></span>|<span data-ttu-id="c2d3e-117">Управление сертификат кодировке Base 64</span><span class="sxs-lookup"><span data-stu-id="c2d3e-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2d3e-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c2d3e-118">Relationships</span></span>
<span data-ttu-id="c2d3e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c2d3e-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c2d3e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2d3e-120">JSON Representation</span></span>
<span data-ttu-id="c2d3e-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2d3e-121">Here is a JSON representation of the resource.</span></span>
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






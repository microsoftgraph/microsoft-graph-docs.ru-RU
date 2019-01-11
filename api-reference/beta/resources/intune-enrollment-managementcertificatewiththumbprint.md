---
title: Тип ресурса managementCertificateWithThumbprint
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d8f18e7fc117f00f99346267f544abc7d12db17e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827218"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="3676f-103">Тип ресурса managementCertificateWithThumbprint</span><span class="sxs-lookup"><span data-stu-id="3676f-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="3676f-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3676f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3676f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3676f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3676f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3676f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3676f-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3676f-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="3676f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3676f-108">Properties</span></span>
|<span data-ttu-id="3676f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3676f-109">Property</span></span>|<span data-ttu-id="3676f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3676f-110">Type</span></span>|<span data-ttu-id="3676f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3676f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3676f-112">отпечаток</span><span class="sxs-lookup"><span data-stu-id="3676f-112">thumbprint</span></span>|<span data-ttu-id="3676f-113">Строка</span><span class="sxs-lookup"><span data-stu-id="3676f-113">String</span></span>|<span data-ttu-id="3676f-114">Отпечаток сертификата, управление</span><span class="sxs-lookup"><span data-stu-id="3676f-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="3676f-115">certificate</span><span class="sxs-lookup"><span data-stu-id="3676f-115">certificate</span></span>|<span data-ttu-id="3676f-116">String</span><span class="sxs-lookup"><span data-stu-id="3676f-116">String</span></span>|<span data-ttu-id="3676f-117">Управление сертификат кодировке Base 64</span><span class="sxs-lookup"><span data-stu-id="3676f-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="3676f-118">Связи</span><span class="sxs-lookup"><span data-stu-id="3676f-118">Relationships</span></span>
<span data-ttu-id="3676f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="3676f-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3676f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3676f-120">JSON Representation</span></span>
<span data-ttu-id="3676f-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3676f-121">Here is a JSON representation of the resource.</span></span>
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






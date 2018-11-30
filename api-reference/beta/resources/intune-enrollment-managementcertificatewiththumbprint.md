---
title: Тип ресурса managementCertificateWithThumbprint
description: Н/Д
ms.openlocfilehash: 320b6241e1ac5a9078ccc32f99f87e9fd337335e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079644"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="02a4b-103">Тип ресурса managementCertificateWithThumbprint</span><span class="sxs-lookup"><span data-stu-id="02a4b-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="02a4b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="02a4b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02a4b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="02a4b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02a4b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="02a4b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02a4b-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="02a4b-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="02a4b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="02a4b-108">Properties</span></span>
|<span data-ttu-id="02a4b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="02a4b-109">Property</span></span>|<span data-ttu-id="02a4b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="02a4b-110">Type</span></span>|<span data-ttu-id="02a4b-111">Description</span><span class="sxs-lookup"><span data-stu-id="02a4b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02a4b-112">отпечаток</span><span class="sxs-lookup"><span data-stu-id="02a4b-112">thumbprint</span></span>|<span data-ttu-id="02a4b-113">String</span><span class="sxs-lookup"><span data-stu-id="02a4b-113">String</span></span>|<span data-ttu-id="02a4b-114">Отпечаток сертификата, управление</span><span class="sxs-lookup"><span data-stu-id="02a4b-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="02a4b-115">certificate</span><span class="sxs-lookup"><span data-stu-id="02a4b-115">certificate</span></span>|<span data-ttu-id="02a4b-116">String</span><span class="sxs-lookup"><span data-stu-id="02a4b-116">String</span></span>|<span data-ttu-id="02a4b-117">Управление сертификат кодировке Base 64</span><span class="sxs-lookup"><span data-stu-id="02a4b-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="02a4b-118">Связи</span><span class="sxs-lookup"><span data-stu-id="02a4b-118">Relationships</span></span>
<span data-ttu-id="02a4b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="02a4b-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="02a4b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02a4b-120">JSON Representation</span></span>
<span data-ttu-id="02a4b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02a4b-121">Here is a JSON representation of the resource.</span></span>
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






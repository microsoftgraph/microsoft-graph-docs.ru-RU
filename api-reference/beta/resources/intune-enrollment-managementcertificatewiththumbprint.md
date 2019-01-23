---
title: Тип ресурса managementCertificateWithThumbprint
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 765d3b9370e4b0f5eda481883956c72bf261e65a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418857"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="a5b40-103">Тип ресурса managementCertificateWithThumbprint</span><span class="sxs-lookup"><span data-stu-id="a5b40-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="a5b40-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a5b40-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a5b40-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5b40-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5b40-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a5b40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5b40-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="a5b40-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a5b40-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5b40-108">Properties</span></span>
|<span data-ttu-id="a5b40-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5b40-109">Property</span></span>|<span data-ttu-id="a5b40-110">Тип</span><span class="sxs-lookup"><span data-stu-id="a5b40-110">Type</span></span>|<span data-ttu-id="a5b40-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a5b40-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5b40-112">отпечаток</span><span class="sxs-lookup"><span data-stu-id="a5b40-112">thumbprint</span></span>|<span data-ttu-id="a5b40-113">String</span><span class="sxs-lookup"><span data-stu-id="a5b40-113">String</span></span>|<span data-ttu-id="a5b40-114">Отпечаток сертификата, управление</span><span class="sxs-lookup"><span data-stu-id="a5b40-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="a5b40-115">certificate</span><span class="sxs-lookup"><span data-stu-id="a5b40-115">certificate</span></span>|<span data-ttu-id="a5b40-116">String</span><span class="sxs-lookup"><span data-stu-id="a5b40-116">String</span></span>|<span data-ttu-id="a5b40-117">Управление сертификат кодировке Base 64</span><span class="sxs-lookup"><span data-stu-id="a5b40-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5b40-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="a5b40-118">Relationships</span></span>
<span data-ttu-id="a5b40-119">Нет</span><span class="sxs-lookup"><span data-stu-id="a5b40-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5b40-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5b40-120">JSON Representation</span></span>
<span data-ttu-id="a5b40-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5b40-121">Here is a JSON representation of the resource.</span></span>
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





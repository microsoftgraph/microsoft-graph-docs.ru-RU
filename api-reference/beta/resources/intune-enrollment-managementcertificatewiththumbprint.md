---
title: Тип ресурса Манажементцертификатевиссумбпринт
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36adab8de1cebe884f6932e2a99b3aba9174d518
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151263"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="87d59-103">Тип ресурса Манажементцертификатевиссумбпринт</span><span class="sxs-lookup"><span data-stu-id="87d59-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="87d59-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="87d59-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87d59-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="87d59-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87d59-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="87d59-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="87d59-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="87d59-107">Properties</span></span>
|<span data-ttu-id="87d59-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="87d59-108">Property</span></span>|<span data-ttu-id="87d59-109">Тип</span><span class="sxs-lookup"><span data-stu-id="87d59-109">Type</span></span>|<span data-ttu-id="87d59-110">Описание</span><span class="sxs-lookup"><span data-stu-id="87d59-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87d59-111">отпечаток</span><span class="sxs-lookup"><span data-stu-id="87d59-111">thumbprint</span></span>|<span data-ttu-id="87d59-112">String</span><span class="sxs-lookup"><span data-stu-id="87d59-112">String</span></span>|<span data-ttu-id="87d59-113">Отпечаток сертификата управления</span><span class="sxs-lookup"><span data-stu-id="87d59-113">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="87d59-114">certificate</span><span class="sxs-lookup"><span data-stu-id="87d59-114">certificate</span></span>|<span data-ttu-id="87d59-115">String</span><span class="sxs-lookup"><span data-stu-id="87d59-115">String</span></span>|<span data-ttu-id="87d59-116">Сертификат управления Base 64 с шифрованием</span><span class="sxs-lookup"><span data-stu-id="87d59-116">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="87d59-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="87d59-117">Relationships</span></span>
<span data-ttu-id="87d59-118">Нет</span><span class="sxs-lookup"><span data-stu-id="87d59-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87d59-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="87d59-119">JSON Representation</span></span>
<span data-ttu-id="87d59-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="87d59-120">Here is a JSON representation of the resource.</span></span>
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





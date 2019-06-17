---
title: Тип ресурса Манажементцертификатевиссумбпринт
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f497780f9ccd21ea608a8c7e56e6926d79263e24
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34963480"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="7b2b7-103">Тип ресурса Манажементцертификатевиссумбпринт</span><span class="sxs-lookup"><span data-stu-id="7b2b7-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="7b2b7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b2b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7b2b7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7b2b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b2b7-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="7b2b7-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="7b2b7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b2b7-107">Properties</span></span>
|<span data-ttu-id="7b2b7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b2b7-108">Property</span></span>|<span data-ttu-id="7b2b7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7b2b7-109">Type</span></span>|<span data-ttu-id="7b2b7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7b2b7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7b2b7-111">отпечаток</span><span class="sxs-lookup"><span data-stu-id="7b2b7-111">thumbprint</span></span>|<span data-ttu-id="7b2b7-112">String</span><span class="sxs-lookup"><span data-stu-id="7b2b7-112">String</span></span>|<span data-ttu-id="7b2b7-113">Отпечаток сертификата управления</span><span class="sxs-lookup"><span data-stu-id="7b2b7-113">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="7b2b7-114">certificate</span><span class="sxs-lookup"><span data-stu-id="7b2b7-114">certificate</span></span>|<span data-ttu-id="7b2b7-115">String</span><span class="sxs-lookup"><span data-stu-id="7b2b7-115">String</span></span>|<span data-ttu-id="7b2b7-116">Сертификат управления Base 64 с шифрованием</span><span class="sxs-lookup"><span data-stu-id="7b2b7-116">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="7b2b7-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="7b2b7-117">Relationships</span></span>
<span data-ttu-id="7b2b7-118">Нет</span><span class="sxs-lookup"><span data-stu-id="7b2b7-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b2b7-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7b2b7-119">JSON Representation</span></span>
<span data-ttu-id="7b2b7-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b2b7-120">Here is a JSON representation of the resource.</span></span>
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






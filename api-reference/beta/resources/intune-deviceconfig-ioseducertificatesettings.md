---
title: Тип ресурса iosEduCertificateSettings
description: Доверенные корневые папки и PFX сертификаты для iOS EDU.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8c48883caa9479638b1a727272abdd0bc5762db9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948677"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="5277a-103">Тип ресурса iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="5277a-103">iosEduCertificateSettings resource type</span></span>

> <span data-ttu-id="5277a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5277a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5277a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5277a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5277a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="5277a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5277a-107">Доверенные корневые папки и PFX сертификаты для iOS EDU.</span><span class="sxs-lookup"><span data-stu-id="5277a-107">Trusted Root and PFX certificates for iOS EDU.</span></span>
## <a name="properties"></a><span data-ttu-id="5277a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5277a-108">Properties</span></span>
|<span data-ttu-id="5277a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5277a-109">Property</span></span>|<span data-ttu-id="5277a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5277a-110">Type</span></span>|<span data-ttu-id="5277a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5277a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5277a-112">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="5277a-112">trustedRootCertificate</span></span>|<span data-ttu-id="5277a-113">Binary</span><span class="sxs-lookup"><span data-stu-id="5277a-113">Binary</span></span>|<span data-ttu-id="5277a-114">Доверенного корневого сертификата.</span><span class="sxs-lookup"><span data-stu-id="5277a-114">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="5277a-115">certFileName</span><span class="sxs-lookup"><span data-stu-id="5277a-115">certFileName</span></span>|<span data-ttu-id="5277a-116">Строка</span><span class="sxs-lookup"><span data-stu-id="5277a-116">String</span></span>|<span data-ttu-id="5277a-117">Имя файла для отображения в пользовательском Интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="5277a-117">File name to display in UI.</span></span>|
|<span data-ttu-id="5277a-118">certificationAuthority</span><span class="sxs-lookup"><span data-stu-id="5277a-118">certificationAuthority</span></span>|<span data-ttu-id="5277a-119">Строка</span><span class="sxs-lookup"><span data-stu-id="5277a-119">String</span></span>|<span data-ttu-id="5277a-120">PKCS центром сертификации.</span><span class="sxs-lookup"><span data-stu-id="5277a-120">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="5277a-121">certificationAuthorityName</span><span class="sxs-lookup"><span data-stu-id="5277a-121">certificationAuthorityName</span></span>|<span data-ttu-id="5277a-122">Строка</span><span class="sxs-lookup"><span data-stu-id="5277a-122">String</span></span>|<span data-ttu-id="5277a-123">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="5277a-123">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="5277a-124">certificateTemplateName</span><span class="sxs-lookup"><span data-stu-id="5277a-124">certificateTemplateName</span></span>|<span data-ttu-id="5277a-125">Строка</span><span class="sxs-lookup"><span data-stu-id="5277a-125">String</span></span>|<span data-ttu-id="5277a-126">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="5277a-126">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="5277a-127">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="5277a-127">renewalThresholdPercentage</span></span>|<span data-ttu-id="5277a-128">Int32</span><span class="sxs-lookup"><span data-stu-id="5277a-128">Int32</span></span>|<span data-ttu-id="5277a-129">Процентное пороговое значение Продление сертификата.</span><span class="sxs-lookup"><span data-stu-id="5277a-129">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="5277a-130">Допустимые значения от 1 до 99</span><span class="sxs-lookup"><span data-stu-id="5277a-130">Valid values 1 to 99</span></span>|
|<span data-ttu-id="5277a-131">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="5277a-131">certificateValidityPeriodValue</span></span>|<span data-ttu-id="5277a-132">Int32</span><span class="sxs-lookup"><span data-stu-id="5277a-132">Int32</span></span>|<span data-ttu-id="5277a-133">Значение срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="5277a-133">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="5277a-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5277a-134">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="5277a-135">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="5277a-135">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="5277a-136">Масштаб срок действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="5277a-136">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="5277a-137">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="5277a-137">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5277a-138">Связи</span><span class="sxs-lookup"><span data-stu-id="5277a-138">Relationships</span></span>
<span data-ttu-id="5277a-139">Нет</span><span class="sxs-lookup"><span data-stu-id="5277a-139">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5277a-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5277a-140">JSON Representation</span></span>
<span data-ttu-id="5277a-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5277a-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosEduCertificateSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEduCertificateSettings",
  "trustedRootCertificate": "binary",
  "certFileName": "String",
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificateTemplateName": "String",
  "renewalThresholdPercentage": 1024,
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String"
}
```






---
title: Тип ресурса Иоседуцертификатесеттингс
description: Доверенные корневые сертификаты и сертификаты PFX для iOS EDU.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b7c3c545f65ffd019d4d3eefe672f9a665bbd41f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463020"
---
# <a name="ioseducertificatesettings-resource-type"></a><span data-ttu-id="cdb8e-103">Тип ресурса Иоседуцертификатесеттингс</span><span class="sxs-lookup"><span data-stu-id="cdb8e-103">iosEduCertificateSettings resource type</span></span>

<span data-ttu-id="cdb8e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdb8e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cdb8e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdb8e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdb8e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cdb8e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdb8e-107">Доверенные корневые сертификаты и сертификаты PFX для iOS EDU.</span><span class="sxs-lookup"><span data-stu-id="cdb8e-107">Trusted Root and PFX certificates for iOS EDU.</span></span>

## <a name="properties"></a><span data-ttu-id="cdb8e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cdb8e-108">Properties</span></span>
|<span data-ttu-id="cdb8e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cdb8e-109">Property</span></span>|<span data-ttu-id="cdb8e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cdb8e-110">Type</span></span>|<span data-ttu-id="cdb8e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cdb8e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdb8e-112">trustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="cdb8e-112">trustedRootCertificate</span></span>|<span data-ttu-id="cdb8e-113">Binary</span><span class="sxs-lookup"><span data-stu-id="cdb8e-113">Binary</span></span>|<span data-ttu-id="cdb8e-114">Доверенный корневой сертификат.</span><span class="sxs-lookup"><span data-stu-id="cdb8e-114">Trusted Root Certificate.</span></span>|
|<span data-ttu-id="cdb8e-115">цертфиленаме</span><span class="sxs-lookup"><span data-stu-id="cdb8e-115">certFileName</span></span>|<span data-ttu-id="cdb8e-116">String</span><span class="sxs-lookup"><span data-stu-id="cdb8e-116">String</span></span>|<span data-ttu-id="cdb8e-117">Имя файла, отображаемое в пользовательском интерфейсе.</span><span class="sxs-lookup"><span data-stu-id="cdb8e-117">File name to display in UI.</span></span>|
|<span data-ttu-id="cdb8e-118">цертификатионаусорити</span><span class="sxs-lookup"><span data-stu-id="cdb8e-118">certificationAuthority</span></span>|<span data-ttu-id="cdb8e-119">String</span><span class="sxs-lookup"><span data-stu-id="cdb8e-119">String</span></span>|<span data-ttu-id="cdb8e-120">Центр сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="cdb8e-120">PKCS Certification Authority.</span></span>|
|<span data-ttu-id="cdb8e-121">цертификатионаусоритинаме</span><span class="sxs-lookup"><span data-stu-id="cdb8e-121">certificationAuthorityName</span></span>|<span data-ttu-id="cdb8e-122">String</span><span class="sxs-lookup"><span data-stu-id="cdb8e-122">String</span></span>|<span data-ttu-id="cdb8e-123">Имя центра сертификации PKCS.</span><span class="sxs-lookup"><span data-stu-id="cdb8e-123">PKCS Certification Authority Name.</span></span>|
|<span data-ttu-id="cdb8e-124">цертификатетемплатенаме</span><span class="sxs-lookup"><span data-stu-id="cdb8e-124">certificateTemplateName</span></span>|<span data-ttu-id="cdb8e-125">String</span><span class="sxs-lookup"><span data-stu-id="cdb8e-125">String</span></span>|<span data-ttu-id="cdb8e-126">Имя шаблона сертификата PKCS.</span><span class="sxs-lookup"><span data-stu-id="cdb8e-126">PKCS Certificate Template Name.</span></span>|
|<span data-ttu-id="cdb8e-127">Свойства renewalthresholdpercentage</span><span class="sxs-lookup"><span data-stu-id="cdb8e-127">renewalThresholdPercentage</span></span>|<span data-ttu-id="cdb8e-128">Int32</span><span class="sxs-lookup"><span data-stu-id="cdb8e-128">Int32</span></span>|<span data-ttu-id="cdb8e-129">Пороговое значение возобновления сертификата.</span><span class="sxs-lookup"><span data-stu-id="cdb8e-129">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="cdb8e-130">Допустимые значения — от 1 до 99</span><span class="sxs-lookup"><span data-stu-id="cdb8e-130">Valid values 1 to 99</span></span>|
|<span data-ttu-id="cdb8e-131">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="cdb8e-131">certificateValidityPeriodValue</span></span>|<span data-ttu-id="cdb8e-132">Int32</span><span class="sxs-lookup"><span data-stu-id="cdb8e-132">Int32</span></span>|<span data-ttu-id="cdb8e-133">Значение срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="cdb8e-133">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="cdb8e-134">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="cdb8e-134">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="cdb8e-135">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="cdb8e-135">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="cdb8e-136">Масштаб срока действия сертификата.</span><span class="sxs-lookup"><span data-stu-id="cdb8e-136">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="cdb8e-137">Возможные значения: `days`, `months`, `years`.</span><span class="sxs-lookup"><span data-stu-id="cdb8e-137">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cdb8e-138">Отношения</span><span class="sxs-lookup"><span data-stu-id="cdb8e-138">Relationships</span></span>
<span data-ttu-id="cdb8e-139">Нет</span><span class="sxs-lookup"><span data-stu-id="cdb8e-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cdb8e-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cdb8e-140">JSON Representation</span></span>
<span data-ttu-id="cdb8e-141">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cdb8e-141">Here is a JSON representation of the resource.</span></span>
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




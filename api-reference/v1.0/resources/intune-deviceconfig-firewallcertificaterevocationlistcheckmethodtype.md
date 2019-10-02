---
title: тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе
description: Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 42f470d7f3d8ef29a69ba8f1cd4f76ddc0f77e96
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359273"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="d9fa5-103">тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="d9fa5-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="d9fa5-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d9fa5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9fa5-105">Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод</span><span class="sxs-lookup"><span data-stu-id="d9fa5-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="d9fa5-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="d9fa5-106">Members</span></span>
|<span data-ttu-id="d9fa5-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="d9fa5-107">Member</span></span>|<span data-ttu-id="d9fa5-108">Значение</span><span class="sxs-lookup"><span data-stu-id="d9fa5-108">Value</span></span>|<span data-ttu-id="d9fa5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d9fa5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9fa5-110">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="d9fa5-110">deviceDefault</span></span>|<span data-ttu-id="d9fa5-111">нуль</span><span class="sxs-lookup"><span data-stu-id="d9fa5-111">0</span></span>|<span data-ttu-id="d9fa5-112">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="d9fa5-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="d9fa5-113">none</span><span class="sxs-lookup"><span data-stu-id="d9fa5-113">none</span></span>|<span data-ttu-id="d9fa5-114">1,1</span><span class="sxs-lookup"><span data-stu-id="d9fa5-114">1</span></span>|<span data-ttu-id="d9fa5-115">Не проверять список отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="d9fa5-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="d9fa5-116">произошл</span><span class="sxs-lookup"><span data-stu-id="d9fa5-116">attempt</span></span>|<span data-ttu-id="d9fa5-117">2</span><span class="sxs-lookup"><span data-stu-id="d9fa5-117">2</span></span>|<span data-ttu-id="d9fa5-118">Проверка списка отзыва сертификатов и предоставление сертификата только в том случае, если сертификат подтвержден подтверждением</span><span class="sxs-lookup"><span data-stu-id="d9fa5-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="d9fa5-119">необходимость</span><span class="sxs-lookup"><span data-stu-id="d9fa5-119">require</span></span>|<span data-ttu-id="d9fa5-120">4</span><span class="sxs-lookup"><span data-stu-id="d9fa5-120">3</span></span>|<span data-ttu-id="d9fa5-121">Требовать успешную проверку списка отзыва сертификатов перед предоставлением сертификата</span><span class="sxs-lookup"><span data-stu-id="d9fa5-121">Require a successful CRL check before allowing a certificate</span></span>|





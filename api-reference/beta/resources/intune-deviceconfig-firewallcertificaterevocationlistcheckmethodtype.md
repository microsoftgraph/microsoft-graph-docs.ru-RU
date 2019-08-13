---
title: тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе
description: Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 832df7bfacbbba9643f4e1181f454bc60038ffb0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36338156"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="eaeb1-103">тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="eaeb1-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="eaeb1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eaeb1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eaeb1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eaeb1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eaeb1-106">Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод</span><span class="sxs-lookup"><span data-stu-id="eaeb1-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="eaeb1-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="eaeb1-107">Members</span></span>
|<span data-ttu-id="eaeb1-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="eaeb1-108">Member</span></span>|<span data-ttu-id="eaeb1-109">Значение</span><span class="sxs-lookup"><span data-stu-id="eaeb1-109">Value</span></span>|<span data-ttu-id="eaeb1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eaeb1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaeb1-111">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="eaeb1-111">deviceDefault</span></span>|<span data-ttu-id="eaeb1-112">нуль</span><span class="sxs-lookup"><span data-stu-id="eaeb1-112">0</span></span>|<span data-ttu-id="eaeb1-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="eaeb1-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="eaeb1-114">none</span><span class="sxs-lookup"><span data-stu-id="eaeb1-114">none</span></span>|<span data-ttu-id="eaeb1-115">1,1</span><span class="sxs-lookup"><span data-stu-id="eaeb1-115">1</span></span>|<span data-ttu-id="eaeb1-116">Не проверять список отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="eaeb1-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="eaeb1-117">произошл</span><span class="sxs-lookup"><span data-stu-id="eaeb1-117">attempt</span></span>|<span data-ttu-id="eaeb1-118">2</span><span class="sxs-lookup"><span data-stu-id="eaeb1-118">2</span></span>|<span data-ttu-id="eaeb1-119">Проверка списка отзыва сертификатов и предоставление сертификата только в том случае, если сертификат подтвержден подтверждением</span><span class="sxs-lookup"><span data-stu-id="eaeb1-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="eaeb1-120">необходимость</span><span class="sxs-lookup"><span data-stu-id="eaeb1-120">require</span></span>|<span data-ttu-id="eaeb1-121">4</span><span class="sxs-lookup"><span data-stu-id="eaeb1-121">3</span></span>|<span data-ttu-id="eaeb1-122">Требовать успешную проверку списка отзыва сертификатов перед предоставлением сертификата</span><span class="sxs-lookup"><span data-stu-id="eaeb1-122">Require a successful CRL check before allowing a certificate</span></span>|




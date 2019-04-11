---
title: тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе
description: Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 789ba503887a7200491f3fdc307ccaeb302b3f05
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776789"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="828af-103">тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="828af-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="828af-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="828af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="828af-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="828af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="828af-106">Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод</span><span class="sxs-lookup"><span data-stu-id="828af-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="828af-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="828af-107">Members</span></span>
|<span data-ttu-id="828af-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="828af-108">Member</span></span>|<span data-ttu-id="828af-109">Значение</span><span class="sxs-lookup"><span data-stu-id="828af-109">Value</span></span>|<span data-ttu-id="828af-110">Описание</span><span class="sxs-lookup"><span data-stu-id="828af-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="828af-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="828af-111">deviceDefault</span></span>|<span data-ttu-id="828af-112">нуль</span><span class="sxs-lookup"><span data-stu-id="828af-112">0</span></span>|<span data-ttu-id="828af-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="828af-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="828af-114">нет</span><span class="sxs-lookup"><span data-stu-id="828af-114">none</span></span>|<span data-ttu-id="828af-115">1,1</span><span class="sxs-lookup"><span data-stu-id="828af-115">1</span></span>|<span data-ttu-id="828af-116">Не проверять список отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="828af-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="828af-117">произошл</span><span class="sxs-lookup"><span data-stu-id="828af-117">attempt</span></span>|<span data-ttu-id="828af-118">2</span><span class="sxs-lookup"><span data-stu-id="828af-118">2</span></span>|<span data-ttu-id="828af-119">Проверка списка ОТЗЫВА сертификатов и предоставление сертификата только в том случае, если сертификат подтвержден подтверждением</span><span class="sxs-lookup"><span data-stu-id="828af-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="828af-120">необходимость</span><span class="sxs-lookup"><span data-stu-id="828af-120">require</span></span>|<span data-ttu-id="828af-121">4</span><span class="sxs-lookup"><span data-stu-id="828af-121">3</span></span>|<span data-ttu-id="828af-122">Требовать успешную проверку списка ОТЗЫВА сертификатов перед предоставлением сертификата</span><span class="sxs-lookup"><span data-stu-id="828af-122">Require a successful CRL check before allowing a certificate</span></span>|






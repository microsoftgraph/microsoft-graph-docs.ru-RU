---
title: тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе
description: Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74989961978ddd10f2c14e57cfe31e25ac831703
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170079"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="ad180-103">тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="ad180-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="ad180-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad180-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ad180-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad180-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad180-106">Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод</span><span class="sxs-lookup"><span data-stu-id="ad180-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="ad180-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="ad180-107">Members</span></span>
|<span data-ttu-id="ad180-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="ad180-108">Member</span></span>|<span data-ttu-id="ad180-109">Значение</span><span class="sxs-lookup"><span data-stu-id="ad180-109">Value</span></span>|<span data-ttu-id="ad180-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ad180-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad180-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="ad180-111">deviceDefault</span></span>|<span data-ttu-id="ad180-112">нуль</span><span class="sxs-lookup"><span data-stu-id="ad180-112">0</span></span>|<span data-ttu-id="ad180-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="ad180-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="ad180-114">Нет</span><span class="sxs-lookup"><span data-stu-id="ad180-114">none</span></span>|<span data-ttu-id="ad180-115">1,1</span><span class="sxs-lookup"><span data-stu-id="ad180-115">1</span></span>|<span data-ttu-id="ad180-116">Не проверять список отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="ad180-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="ad180-117">произошл</span><span class="sxs-lookup"><span data-stu-id="ad180-117">attempt</span></span>|<span data-ttu-id="ad180-118">2</span><span class="sxs-lookup"><span data-stu-id="ad180-118">2</span></span>|<span data-ttu-id="ad180-119">Проверка списка ОТЗЫВА сертификатов и предоставление сертификата только в том случае, если сертификат подтвержден подтверждением</span><span class="sxs-lookup"><span data-stu-id="ad180-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="ad180-120">необходимость</span><span class="sxs-lookup"><span data-stu-id="ad180-120">require</span></span>|<span data-ttu-id="ad180-121">4</span><span class="sxs-lookup"><span data-stu-id="ad180-121">3</span></span>|<span data-ttu-id="ad180-122">Требовать успешную проверку списка ОТЗЫВА сертификатов перед предоставлением сертификата</span><span class="sxs-lookup"><span data-stu-id="ad180-122">Require a successful CRL check before allowing a certificate</span></span>|





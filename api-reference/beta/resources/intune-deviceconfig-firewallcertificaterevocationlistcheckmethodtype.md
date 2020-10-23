---
title: тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе
description: Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 84ae3483976b9a6aa5763ba9f2229b4af582c3d9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728986"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="fe695-103">тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="fe695-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="fe695-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe695-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fe695-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe695-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe695-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe695-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe695-107">Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод</span><span class="sxs-lookup"><span data-stu-id="fe695-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="fe695-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="fe695-108">Members</span></span>
|<span data-ttu-id="fe695-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="fe695-109">Member</span></span>|<span data-ttu-id="fe695-110">Значение</span><span class="sxs-lookup"><span data-stu-id="fe695-110">Value</span></span>|<span data-ttu-id="fe695-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fe695-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe695-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="fe695-112">deviceDefault</span></span>|<span data-ttu-id="fe695-113">нуль</span><span class="sxs-lookup"><span data-stu-id="fe695-113">0</span></span>|<span data-ttu-id="fe695-114">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="fe695-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="fe695-115">none</span><span class="sxs-lookup"><span data-stu-id="fe695-115">none</span></span>|<span data-ttu-id="fe695-116">1,1</span><span class="sxs-lookup"><span data-stu-id="fe695-116">1</span></span>|<span data-ttu-id="fe695-117">Не проверять список отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="fe695-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="fe695-118">произошл</span><span class="sxs-lookup"><span data-stu-id="fe695-118">attempt</span></span>|<span data-ttu-id="fe695-119">2</span><span class="sxs-lookup"><span data-stu-id="fe695-119">2</span></span>|<span data-ttu-id="fe695-120">Проверка списка отзыва сертификатов и предоставление сертификата только в том случае, если сертификат подтвержден подтверждением</span><span class="sxs-lookup"><span data-stu-id="fe695-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="fe695-121">необходимость</span><span class="sxs-lookup"><span data-stu-id="fe695-121">require</span></span>|<span data-ttu-id="fe695-122">4</span><span class="sxs-lookup"><span data-stu-id="fe695-122">3</span></span>|<span data-ttu-id="fe695-123">Требовать успешную проверку списка отзыва сертификатов перед предоставлением сертификата</span><span class="sxs-lookup"><span data-stu-id="fe695-123">Require a successful CRL check before allowing a certificate</span></span>|






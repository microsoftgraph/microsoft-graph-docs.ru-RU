---
title: тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе
description: Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3c1c9e4ae9068f6dc9d754da93a30979367e7587
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294503"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="e1417-103">тип перечисления Фиреваллцертификатеревокатионлистчеккмесодтипе</span><span class="sxs-lookup"><span data-stu-id="e1417-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="e1417-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1417-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1417-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1417-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1417-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e1417-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1417-107">Возможные значения для Фиреваллцертификатеревокатионлистчеккмесод</span><span class="sxs-lookup"><span data-stu-id="e1417-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="e1417-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="e1417-108">Members</span></span>
|<span data-ttu-id="e1417-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="e1417-109">Member</span></span>|<span data-ttu-id="e1417-110">Значение</span><span class="sxs-lookup"><span data-stu-id="e1417-110">Value</span></span>|<span data-ttu-id="e1417-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e1417-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1417-112">девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="e1417-112">deviceDefault</span></span>|<span data-ttu-id="e1417-113">нуль</span><span class="sxs-lookup"><span data-stu-id="e1417-113">0</span></span>|<span data-ttu-id="e1417-114">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="e1417-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="e1417-115">Нет</span><span class="sxs-lookup"><span data-stu-id="e1417-115">none</span></span>|<span data-ttu-id="e1417-116">1,1</span><span class="sxs-lookup"><span data-stu-id="e1417-116">1</span></span>|<span data-ttu-id="e1417-117">Не проверять список отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="e1417-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="e1417-118">произошл</span><span class="sxs-lookup"><span data-stu-id="e1417-118">attempt</span></span>|<span data-ttu-id="e1417-119">2</span><span class="sxs-lookup"><span data-stu-id="e1417-119">2</span></span>|<span data-ttu-id="e1417-120">Проверка списка отзыва сертификатов и предоставление сертификата только в том случае, если сертификат подтвержден подтверждением</span><span class="sxs-lookup"><span data-stu-id="e1417-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="e1417-121">необходимость</span><span class="sxs-lookup"><span data-stu-id="e1417-121">require</span></span>|<span data-ttu-id="e1417-122">4</span><span class="sxs-lookup"><span data-stu-id="e1417-122">3</span></span>|<span data-ttu-id="e1417-123">Требовать успешную проверку списка отзыва сертификатов перед предоставлением сертификата</span><span class="sxs-lookup"><span data-stu-id="e1417-123">Require a successful CRL check before allowing a certificate</span></span>|





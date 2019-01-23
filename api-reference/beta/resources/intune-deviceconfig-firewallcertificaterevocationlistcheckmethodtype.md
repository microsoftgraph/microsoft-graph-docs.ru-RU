---
title: Тип перечисления firewallCertificateRevocationListCheckMethodType
description: Возможные значения для firewallCertificateRevocationListCheckMethod
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4585c30c0a910befd8df8482636916af9ad9c0d6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396415"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="12481-103">Тип перечисления firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="12481-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="12481-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="12481-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="12481-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="12481-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12481-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="12481-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12481-107">Возможные значения для firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="12481-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="12481-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="12481-108">Members</span></span>
|<span data-ttu-id="12481-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="12481-109">Member</span></span>|<span data-ttu-id="12481-110">Значение</span><span class="sxs-lookup"><span data-stu-id="12481-110">Value</span></span>|<span data-ttu-id="12481-111">Описание</span><span class="sxs-lookup"><span data-stu-id="12481-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12481-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="12481-112">deviceDefault</span></span>|<span data-ttu-id="12481-113">0</span><span class="sxs-lookup"><span data-stu-id="12481-113">0</span></span>|<span data-ttu-id="12481-114">Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="12481-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="12481-115">none</span><span class="sxs-lookup"><span data-stu-id="12481-115">none</span></span>|<span data-ttu-id="12481-116">1</span><span class="sxs-lookup"><span data-stu-id="12481-116">1</span></span>|<span data-ttu-id="12481-117">Не проверять списка отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="12481-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="12481-118">Попытка</span><span class="sxs-lookup"><span data-stu-id="12481-118">attempt</span></span>|<span data-ttu-id="12481-119">2</span><span class="sxs-lookup"><span data-stu-id="12481-119">2</span></span>|<span data-ttu-id="12481-120">Попытайтесь проверки списка отзыва Сертификатов и разрешить сертификат только в том случае, если сертификат подтверждается при проверке</span><span class="sxs-lookup"><span data-stu-id="12481-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="12481-121">Требовать</span><span class="sxs-lookup"><span data-stu-id="12481-121">require</span></span>|<span data-ttu-id="12481-122">3</span><span class="sxs-lookup"><span data-stu-id="12481-122">3</span></span>|<span data-ttu-id="12481-123">Требовать успешной проверки списка отзыва Сертификатов, перед тем как разрешить сертификата</span><span class="sxs-lookup"><span data-stu-id="12481-123">Require a successful CRL check before allowing a certificate</span></span>|





---
title: Тип перечисления firewallCertificateRevocationListCheckMethodType
description: Возможные значения для firewallCertificateRevocationListCheckMethod
author: tfitzmac
ms.openlocfilehash: ab496b5deb8f096bdc48a2b50a1af994c8ec8d5b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27353664"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="951f6-103">Тип перечисления firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="951f6-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="951f6-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="951f6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="951f6-105">Возможные значения для firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="951f6-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="951f6-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="951f6-106">Members</span></span>
|<span data-ttu-id="951f6-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="951f6-107">Member</span></span>|<span data-ttu-id="951f6-108">Значение</span><span class="sxs-lookup"><span data-stu-id="951f6-108">Value</span></span>|<span data-ttu-id="951f6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="951f6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="951f6-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="951f6-110">deviceDefault</span></span>|<span data-ttu-id="951f6-111">0</span><span class="sxs-lookup"><span data-stu-id="951f6-111">0</span></span>|<span data-ttu-id="951f6-112">Значение не настраивается с Intune, не переопределяют настраиваемых пользователем устройства по умолчанию</span><span class="sxs-lookup"><span data-stu-id="951f6-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="951f6-113">none</span><span class="sxs-lookup"><span data-stu-id="951f6-113">none</span></span>|<span data-ttu-id="951f6-114">1</span><span class="sxs-lookup"><span data-stu-id="951f6-114">1</span></span>|<span data-ttu-id="951f6-115">Не проверять списка отзыва сертификатов</span><span class="sxs-lookup"><span data-stu-id="951f6-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="951f6-116">Попытка</span><span class="sxs-lookup"><span data-stu-id="951f6-116">attempt</span></span>|<span data-ttu-id="951f6-117">2</span><span class="sxs-lookup"><span data-stu-id="951f6-117">2</span></span>|<span data-ttu-id="951f6-118">Попытайтесь проверки списка отзыва Сертификатов и разрешить сертификат только в том случае, если сертификат подтверждается при проверке</span><span class="sxs-lookup"><span data-stu-id="951f6-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="951f6-119">Требовать</span><span class="sxs-lookup"><span data-stu-id="951f6-119">require</span></span>|<span data-ttu-id="951f6-120">3</span><span class="sxs-lookup"><span data-stu-id="951f6-120">3</span></span>|<span data-ttu-id="951f6-121">Требовать успешной проверки списка отзыва Сертификатов, перед тем как разрешить сертификата</span><span class="sxs-lookup"><span data-stu-id="951f6-121">Require a successful CRL check before allowing a certificate</span></span>|




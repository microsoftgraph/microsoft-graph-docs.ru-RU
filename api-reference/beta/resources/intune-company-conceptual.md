---
title: Корпоративные условия в Microsoft Intune
description: Вы можете развернуть условия Intune для групп пользователей, чтобы показать, как регистрация, доступ к рабочим ресурсам и приложение "Корпоративный портал" влияют на устройства и пользователей. Пользователи должны принять условия, чтобы использовать Корпоративный портал для регистрации и доступа к своей рабочей среде.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: eb7221a8a04c35d92f04678369ff690245122f97
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931533"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a><span data-ttu-id="f8cc3-104">Корпоративные условия в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f8cc3-104">Company terms and conditions in Microsoft Intune</span></span>

> <span data-ttu-id="f8cc3-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="f8cc3-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8cc3-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f8cc3-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8cc3-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f8cc3-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="f8cc3-108">Вы можете развернуть условия Intune для групп пользователей, чтобы показать, как регистрация, доступ к рабочим ресурсам и приложение "Корпоративный портал" влияют на устройства и пользователей.</span><span class="sxs-lookup"><span data-stu-id="f8cc3-108">You can deploy Intune terms and conditions to user groups to explain how enrollment, access to work resources, and the Company Portal app affect devices and users.</span></span> <span data-ttu-id="f8cc3-109">Пользователи должны принять условия, чтобы использовать Корпоративный портал для регистрации и доступа к своей рабочей среде.</span><span class="sxs-lookup"><span data-stu-id="f8cc3-109">Users must accept the terms and conditions before they can use the Company Portal to enroll and access their work.</span></span>

<span data-ttu-id="f8cc3-110">Можно создать и развернуть несколько политик с различными условиями.</span><span class="sxs-lookup"><span data-stu-id="f8cc3-110">You can create and deploy multiple policies containing different terms and conditions.</span></span> <span data-ttu-id="f8cc3-111">Вы также можете создать версии одних условий на разных языках, а затем развернуть их в соответствующих группах.</span><span class="sxs-lookup"><span data-stu-id="f8cc3-111">You can also produce versions of the same terms and conditions in different languages and then deploy these to their appropriate groups.</span></span>

<span data-ttu-id="f8cc3-112">Для управления корпоративными условиями в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="f8cc3-112">The following Graph resources are available to manage company terms and conditions in Intune:</span></span>

- [<span data-ttu-id="f8cc3-113">Условия</span><span class="sxs-lookup"><span data-stu-id="f8cc3-113">Terms and conditions</span></span>](intune-companyterms-termsandconditions.md)
- [<span data-ttu-id="f8cc3-114">Состояние принятия условий</span><span class="sxs-lookup"><span data-stu-id="f8cc3-114">Terms and conditions acceptance status</span></span>](intune-companyterms-termsandconditionsacceptancestatus.md)
- [<span data-ttu-id="f8cc3-115">Назначение условий</span><span class="sxs-lookup"><span data-stu-id="f8cc3-115">Terms and conditions assignment</span></span>](intune-companyterms-termsandconditionsassignment.md)
- [<span data-ttu-id="f8cc3-116">Назначение группы сроками и условиями</span><span class="sxs-lookup"><span data-stu-id="f8cc3-116">Terms and conditions group assignment</span></span>](intune-companyterms-termsandconditionsgroupassignment.md)

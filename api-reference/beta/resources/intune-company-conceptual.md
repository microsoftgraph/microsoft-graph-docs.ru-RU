---
title: Условия и условия компании в Microsoft Intune — API Microsoft Graph
description: Список API Microsoft Graph для конечных точек Intune (REST), определяющих термины и условия для организации клиента.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 1277a6893ddd306b7050fafc70b815217d376b14
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32557805"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a><span data-ttu-id="0207f-103">Корпоративные условия в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0207f-103">Company terms and conditions in Microsoft Intune</span></span>

> <span data-ttu-id="0207f-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0207f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0207f-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0207f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0207f-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0207f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="0207f-107">Вы можете развернуть условия Intune для групп пользователей, чтобы показать, как регистрация, доступ к рабочим ресурсам и приложение "Корпоративный портал" влияют на устройства и пользователей.</span><span class="sxs-lookup"><span data-stu-id="0207f-107">You can deploy Intune terms and conditions to user groups to explain how enrollment, access to work resources, and the Company Portal app affect devices and users.</span></span> <span data-ttu-id="0207f-108">Пользователи должны принять условия, чтобы использовать Корпоративный портал для регистрации и доступа к своей рабочей среде.</span><span class="sxs-lookup"><span data-stu-id="0207f-108">Users must accept the terms and conditions before they can use the Company Portal to enroll and access their work.</span></span>

<span data-ttu-id="0207f-109">Можно создать и развернуть несколько политик с различными условиями.</span><span class="sxs-lookup"><span data-stu-id="0207f-109">You can create and deploy multiple policies containing different terms and conditions.</span></span> <span data-ttu-id="0207f-110">Вы также можете создать версии одних условий на разных языках, а затем развернуть их в соответствующих группах.</span><span class="sxs-lookup"><span data-stu-id="0207f-110">You can also produce versions of the same terms and conditions in different languages and then deploy these to their appropriate groups.</span></span>

<span data-ttu-id="0207f-111">Для управления корпоративными условиями в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="0207f-111">The following Graph resources are available to manage company terms and conditions in Intune:</span></span>

- [<span data-ttu-id="0207f-112">Условия</span><span class="sxs-lookup"><span data-stu-id="0207f-112">Terms and conditions</span></span>](intune-companyterms-termsandconditions.md)
- [<span data-ttu-id="0207f-113">Состояние принятия условий</span><span class="sxs-lookup"><span data-stu-id="0207f-113">Terms and conditions acceptance status</span></span>](intune-companyterms-termsandconditionsacceptancestatus.md)
- [<span data-ttu-id="0207f-114">Назначение условий</span><span class="sxs-lookup"><span data-stu-id="0207f-114">Terms and conditions assignment</span></span>](intune-companyterms-termsandconditionsassignment.md)
- [<span data-ttu-id="0207f-115">Назначение групп условий</span><span class="sxs-lookup"><span data-stu-id="0207f-115">Terms and conditions group assignment</span></span>](intune-companyterms-termsandconditionsgroupassignment.md)

---
title: Условия и условия компании в Microsoft Intune — API Microsoft Graph
description: Список API Microsoft Graph для конечных точек Intune (REST), определяющих термины и условия для организации клиента.
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: c10487c6d708c3c8f7868abd07a629084b6447c2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989506"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a><span data-ttu-id="b3433-103">Корпоративные условия в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b3433-103">Company terms and conditions in Microsoft Intune</span></span>

> <span data-ttu-id="b3433-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b3433-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3433-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3433-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3433-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b3433-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3433-107">Вы можете развернуть условия Intune для групп пользователей, чтобы показать, как регистрация, доступ к рабочим ресурсам и приложение "Корпоративный портал" влияют на устройства и пользователей.</span><span class="sxs-lookup"><span data-stu-id="b3433-107">You can deploy Intune terms and conditions to user groups to explain how enrollment, access to work resources, and the Company Portal app affect devices and users.</span></span> <span data-ttu-id="b3433-108">Пользователи должны принять условия, чтобы использовать Корпоративный портал для регистрации и доступа к своей рабочей среде.</span><span class="sxs-lookup"><span data-stu-id="b3433-108">Users must accept the terms and conditions before they can use the Company Portal to enroll and access their work.</span></span>

<span data-ttu-id="b3433-109">Можно создать и развернуть несколько политик с различными условиями.</span><span class="sxs-lookup"><span data-stu-id="b3433-109">You can create and deploy multiple policies containing different terms and conditions.</span></span> <span data-ttu-id="b3433-110">Вы также можете создать версии одних условий на разных языках, а затем развернуть их в соответствующих группах.</span><span class="sxs-lookup"><span data-stu-id="b3433-110">You can also produce versions of the same terms and conditions in different languages and then deploy these to their appropriate groups.</span></span>

<span data-ttu-id="b3433-111">Для управления корпоративными условиями в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="b3433-111">The following Graph resources are available to manage company terms and conditions in Intune:</span></span>

- [<span data-ttu-id="b3433-112">Условия</span><span class="sxs-lookup"><span data-stu-id="b3433-112">Terms and conditions</span></span>](intune-companyterms-termsandconditions.md)
- [<span data-ttu-id="b3433-113">Состояние принятия условий</span><span class="sxs-lookup"><span data-stu-id="b3433-113">Terms and conditions acceptance status</span></span>](intune-companyterms-termsandconditionsacceptancestatus.md)
- [<span data-ttu-id="b3433-114">Назначение условий</span><span class="sxs-lookup"><span data-stu-id="b3433-114">Terms and conditions assignment</span></span>](intune-companyterms-termsandconditionsassignment.md)
- [<span data-ttu-id="b3433-115">Назначение групп условий</span><span class="sxs-lookup"><span data-stu-id="b3433-115">Terms and conditions group assignment</span></span>](intune-companyterms-termsandconditionsgroupassignment.md)

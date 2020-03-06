---
title: Условия и условия компании в Microsoft Intune — API Microsoft Graph
description: Перечисление конечных точек API Microsoft Graph для Intune (REST), которые поддерживают условия и условия компании.
localization_priority: Normal
author: davidmu1
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: a0d6e64e8423896c5a506886f7f4cdc3c70ded11
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532691"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a><span data-ttu-id="6be63-103">Корпоративные условия в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6be63-103">Company terms and conditions in Microsoft Intune</span></span>

<span data-ttu-id="6be63-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6be63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6be63-105">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6be63-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="6be63-106">Вы можете развернуть условия Intune для групп пользователей, чтобы показать, как регистрация, доступ к рабочим ресурсам и приложение "Корпоративный портал" влияют на устройства и пользователей.</span><span class="sxs-lookup"><span data-stu-id="6be63-106">You can deploy Intune terms and conditions to user groups to explain how enrollment, access to work resources, and the Company Portal app affect devices and users.</span></span> <span data-ttu-id="6be63-107">Пользователи должны принять условия, чтобы использовать Корпоративный портал для регистрации и доступа к своей рабочей среде.</span><span class="sxs-lookup"><span data-stu-id="6be63-107">Users must accept the terms and conditions before they can use the Company Portal to enroll and access their work.</span></span>

<span data-ttu-id="6be63-108">Можно создать и развернуть несколько политик с различными условиями.</span><span class="sxs-lookup"><span data-stu-id="6be63-108">You can create and deploy multiple policies containing different terms and conditions.</span></span> <span data-ttu-id="6be63-109">Вы также можете создать версии одних условий на разных языках, а затем развернуть их в соответствующих группах.</span><span class="sxs-lookup"><span data-stu-id="6be63-109">You can also produce versions of the same terms and conditions in different languages and then deploy these to their appropriate groups.</span></span>

<span data-ttu-id="6be63-110">Для управления корпоративными условиями в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="6be63-110">The following Graph resources are available to manage company terms and conditions in Intune:</span></span>

- [<span data-ttu-id="6be63-111">Условия</span><span class="sxs-lookup"><span data-stu-id="6be63-111">Terms and conditions</span></span>](intune-companyterms-termsandconditions.md)
- [<span data-ttu-id="6be63-112">Состояние принятия условий</span><span class="sxs-lookup"><span data-stu-id="6be63-112">Terms and conditions acceptance status</span></span>](intune-companyterms-termsandconditionsacceptancestatus.md)
- [<span data-ttu-id="6be63-113">Назначение условий</span><span class="sxs-lookup"><span data-stu-id="6be63-113">Terms and conditions assignment</span></span>](intune-companyterms-termsandconditionsassignment.md)


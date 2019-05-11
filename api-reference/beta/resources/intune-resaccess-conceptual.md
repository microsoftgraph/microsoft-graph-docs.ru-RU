---
title: Управление сертификатами доступа к ресурсам в Intune — API Microsoft Graph
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), которые управляют сертификатами доступа к ресурсам для организации клиента.
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c2af10e3f45e59ec9bac83fb71a8220e37e769c2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939940"
---
# <a name="manage-resource-access-certificates-in-intune"></a><span data-ttu-id="ede5e-103">Управление сертификатами доступа к ресурсам в Intune</span><span class="sxs-lookup"><span data-stu-id="ede5e-103">Manage resource access certificates in Intune</span></span>

> <span data-ttu-id="ede5e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ede5e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ede5e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ede5e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ede5e-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ede5e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="ede5e-107">Вы можете импортировать PFX-сертификаты с помощью API Microsoft Graph для Intune.</span><span class="sxs-lookup"><span data-stu-id="ede5e-107">You can import PFX certificates using Microsoft Graph API for Intune.</span></span>

<span data-ttu-id="ede5e-108">Для управления регистрацией в Intune используются перечисленные ниже ресурсы Graph.</span><span class="sxs-lookup"><span data-stu-id="ede5e-108">The following Graph resources are available to manage enrollment in Intune:</span></span>

- [<span data-ttu-id="ede5e-109">Сертификат PFX пользователя</span><span class="sxs-lookup"><span data-stu-id="ede5e-109">User PFX certificate</span></span>](intune-raimportcerts-userpfxcertificate.md)
- [<span data-ttu-id="ede5e-110">Предполагаемое назначение PFX пользователя</span><span class="sxs-lookup"><span data-stu-id="ede5e-110">User PFX intended purpose</span></span>](intune-raimportcerts-userpfxintendedpurpose.md)
- [<span data-ttu-id="ede5e-111">Схема заполнения пользователя PFX</span><span class="sxs-lookup"><span data-stu-id="ede5e-111">User PFX padding scheme</span></span>](intune-raimportcerts-userpfxpaddingscheme.md)

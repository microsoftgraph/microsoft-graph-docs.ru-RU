---
title: Управление доступом на основе ролей в Microsoft Intune
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), которые определяют управление доступом на основе ролей (RBAC) для организации клиента и управляют им.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 24280426585014f5e397dab39daa71f8930b26c4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566390"
---
# <a name="role-based-access-control-in-microsoft-intune"></a><span data-ttu-id="bc7ab-103">Управление доступом на основе ролей в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="bc7ab-103">Role-based access control in Microsoft Intune</span></span>

> <span data-ttu-id="bc7ab-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bc7ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc7ab-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc7ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc7ab-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bc7ab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="bc7ab-107">Управление доступом на основе ролей в Intune определяет, кто может выполнять действия с объектами Intune и вносить изменения в управляемые приложения, устройства и сведения о пользователях.</span><span class="sxs-lookup"><span data-stu-id="bc7ab-107">Intune's role-based access control determines who can perform actions on Intune objects and make changes for managed applications, users and devices.</span></span>   

<span data-ttu-id="bc7ab-108">Следующие ресурсы Graph помогут в управлении доступом на основе ролей в Intune:</span><span class="sxs-lookup"><span data-stu-id="bc7ab-108">The following Graph resources are available to manage role-based access control in Intune:</span></span>

- [<span data-ttu-id="bc7ab-109">Данные назначенной роли для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="bc7ab-109">Device and app management assigned role details</span></span>](intune-rbac-deviceandappmanagementassignedroledetails.md)
- [<span data-ttu-id="bc7ab-110">Назначение роли управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="bc7ab-110">Device and app management role assignment</span></span>](intune-rbac-deviceandappmanagementroleassignment.md)
- [<span data-ttu-id="bc7ab-111">Определение роли управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="bc7ab-111">Device and app management role definition</span></span>](intune-rbac-deviceandappmanagementroledefinition.md)
- [<span data-ttu-id="bc7ab-112">Действие ресурса</span><span class="sxs-lookup"><span data-stu-id="bc7ab-112">Resource action</span></span>](intune-rbac-resourceaction.md)
- [<span data-ttu-id="bc7ab-113">Операция ресурса</span><span class="sxs-lookup"><span data-stu-id="bc7ab-113">Resource operation</span></span>](intune-rbac-resourceoperation.md)
- [<span data-ttu-id="bc7ab-114">Назначение ролей</span><span class="sxs-lookup"><span data-stu-id="bc7ab-114">Role assignment</span></span>](intune-rbac-roleassignment.md)
- [<span data-ttu-id="bc7ab-115">Тип области назначения ролей</span><span class="sxs-lookup"><span data-stu-id="bc7ab-115">Role assignment scope type</span></span>](intune-rbac-roleassignmentscopetype.md)
- [<span data-ttu-id="bc7ab-116">Определение ролей</span><span class="sxs-lookup"><span data-stu-id="bc7ab-116">Role definition</span></span>](intune-rbac-roledefinition.md)
- [<span data-ttu-id="bc7ab-117">Разрешение роли</span><span class="sxs-lookup"><span data-stu-id="bc7ab-117">Role permission</span></span>](intune-rbac-rolepermission.md)
- [<span data-ttu-id="bc7ab-118">Тег области роли</span><span class="sxs-lookup"><span data-stu-id="bc7ab-118">Role scope tag</span></span>](intune-rbac-rolescopetag.md)

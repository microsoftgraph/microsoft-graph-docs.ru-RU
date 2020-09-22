---
title: Управление доступом на основе ролей в Microsoft Intune
description: Перечисляет API Microsoft Graph для конечных точек Intune (REST), которые определяют управление доступом на основе ролей (RBAC) для организации клиента и управляют им.
localization_priority: Normal
author: dougeby
ms.prod: intune
ms.openlocfilehash: a95c71613755cd9853cca4a56d4cd36caf0d7df7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084424"
---
# <a name="role-based-access-control-in-microsoft-intune"></a><span data-ttu-id="c5a5f-103">Управление доступом на основе ролей в Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c5a5f-103">Role-based access control in Microsoft Intune</span></span>

<span data-ttu-id="c5a5f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5a5f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c5a5f-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c5a5f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5a5f-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c5a5f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5a5f-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c5a5f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5a5f-108">Управление доступом на основе ролей в Intune определяет, кто может выполнять действия с объектами Intune и вносить изменения в управляемые приложения, устройства и сведения о пользователях.</span><span class="sxs-lookup"><span data-stu-id="c5a5f-108">Intune's role-based access control determines who can perform actions on Intune objects and make changes for managed applications, users and devices.</span></span>   

<span data-ttu-id="c5a5f-109">Следующие ресурсы Graph помогут в управлении доступом на основе ролей в Intune:</span><span class="sxs-lookup"><span data-stu-id="c5a5f-109">The following Graph resources are available to manage role-based access control in Intune:</span></span>

- [<span data-ttu-id="c5a5f-110">Данные назначенной роли для управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="c5a5f-110">Device and app management assigned role details</span></span>](intune-rbac-deviceandappmanagementassignedroledetails.md)
- [<span data-ttu-id="c5a5f-111">Назначение роли управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="c5a5f-111">Device and app management role assignment</span></span>](intune-rbac-deviceandappmanagementroleassignment.md)
- [<span data-ttu-id="c5a5f-112">Определение роли управления устройствами и приложениями</span><span class="sxs-lookup"><span data-stu-id="c5a5f-112">Device and app management role definition</span></span>](intune-rbac-deviceandappmanagementroledefinition.md)
- [<span data-ttu-id="c5a5f-113">Несколько приложений RBAC</span><span class="sxs-lookup"><span data-stu-id="c5a5f-113">Rbac application multiple</span></span>](intune-rbac-rbacapplicationmultiple.md)
- [<span data-ttu-id="c5a5f-114">Действие ресурса</span><span class="sxs-lookup"><span data-stu-id="c5a5f-114">Resource action</span></span>](intune-rbac-resourceaction.md)
- [<span data-ttu-id="c5a5f-115">Операция ресурса</span><span class="sxs-lookup"><span data-stu-id="c5a5f-115">Resource operation</span></span>](intune-rbac-resourceoperation.md)
- [<span data-ttu-id="c5a5f-116">Назначение ролей</span><span class="sxs-lookup"><span data-stu-id="c5a5f-116">Role assignment</span></span>](intune-rbac-roleassignment.md)
- [<span data-ttu-id="c5a5f-117">Тип области назначения ролей</span><span class="sxs-lookup"><span data-stu-id="c5a5f-117">Role assignment scope type</span></span>](intune-rbac-roleassignmentscopetype.md)
- [<span data-ttu-id="c5a5f-118">Определение ролей</span><span class="sxs-lookup"><span data-stu-id="c5a5f-118">Role definition</span></span>](intune-rbac-roledefinition.md)
- [<span data-ttu-id="c5a5f-119">Управление ролями</span><span class="sxs-lookup"><span data-stu-id="c5a5f-119">Role management</span></span>](intune-rbac-rolemanagement.md)
- [<span data-ttu-id="c5a5f-120">Разрешение роли</span><span class="sxs-lookup"><span data-stu-id="c5a5f-120">Role permission</span></span>](intune-rbac-rolepermission.md)
- [<span data-ttu-id="c5a5f-121">Тег области роли</span><span class="sxs-lookup"><span data-stu-id="c5a5f-121">Role scope tag</span></span>](intune-rbac-rolescopetag.md)
- [<span data-ttu-id="c5a5f-122">Автоматическое назначение тега области применения роли</span><span class="sxs-lookup"><span data-stu-id="c5a5f-122">Role scope tag auto assignment</span></span>](intune-rbac-rolescopetagautoassignment.md)



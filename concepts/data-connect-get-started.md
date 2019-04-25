---
title: Начало работы с подключением данных Microsoft Graph (предварительная версия)
description: 'Прежде чем использовать подключение данных Microsoft Graph, администратору Office 365 необходимо выполнить два действия, которые включают возможность управления перемещением данных для администраторов через Privileged Access Management (PAM). '
author: ajacks-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: f7426147908a2ded298bee065c05afffc182cd4b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526121"
---
# <a name="get-started-with-microsoft-graph-data-connect-preview"></a><span data-ttu-id="2e3c3-103">Начало работы с подключением данных Microsoft Graph (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="2e3c3-103">Get started with Microsoft Graph data connect (preview)</span></span>

<span data-ttu-id="2e3c3-104">Прежде чем использовать подключение данных Microsoft Graph, администратору Office 365 необходимо выполнить два действия, которые включают возможность управления перемещением данных для администраторов через Privileged Access Management (PAM).</span><span class="sxs-lookup"><span data-stu-id="2e3c3-104">Before you can use Microsoft Graph data connect, an Office 365 administrator must take two actions, both of which enable the ability for the admin to control data movement through Privileged Access Management (PAM).</span></span> 

1. <span data-ttu-id="2e3c3-105">Дайте согласие на участие в подключении данных Microsoft Graph через портал администрирования Microsoft 365 на странице **Службы и надстройки**.</span><span class="sxs-lookup"><span data-stu-id="2e3c3-105">Give consent to opt in to Microsoft Graph data connect through the Microsoft 365 Admin Portal, on the **Services & add-ins** page.</span></span> <span data-ttu-id="2e3c3-106">Это позволит Microsoft Azure осуществлять запросы на перемещение данных (вы сохраните полный контроль над данными, но разрешите ресурсам Azure доступ к ним).</span><span class="sxs-lookup"><span data-stu-id="2e3c3-106">This will allow data movement requests to Microsoft Azure (that is, keep full control over the data, but allow Azure resources to access it).</span></span> <span data-ttu-id="2e3c3-107">Данные не будут передаваться, пока не будет утвержден определенный конвейер.</span><span class="sxs-lookup"><span data-stu-id="2e3c3-107">No data is transferred unless approval for a specific pipeline is provided later.</span></span>
2. <span data-ttu-id="2e3c3-108">Настройте утверждающую группу в подписке Office 365.</span><span class="sxs-lookup"><span data-stu-id="2e3c3-108">Set an approver group within the Office 365 subscription.</span></span> <span data-ttu-id="2e3c3-109">Убедитесь, что утверждающая группа не пустая.</span><span class="sxs-lookup"><span data-stu-id="2e3c3-109">Make sure that the approver group is not empty.</span></span> <span data-ttu-id="2e3c3-110">Только пользователи в группе могут утверждать запросы на перемещение данных.</span><span class="sxs-lookup"><span data-stu-id="2e3c3-110">Only the users in the group can approve data movement requests.</span></span>

<span data-ttu-id="2e3c3-111">Чтобы узнать подробные пошаговые инструкции, см. [учебный модуль по подключению данных в Microsoft Graph](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md).</span><span class="sxs-lookup"><span data-stu-id="2e3c3-111">For detailed step-by-step instructions, see the [Microsoft Graph data connect training module](https://github.com/microsoftgraph/msgraph-training-dataconnect/blob/master/Lab.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="2e3c3-112">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="2e3c3-112">Next steps</span></span>

<span data-ttu-id="2e3c3-113">Поздравляем!</span><span class="sxs-lookup"><span data-stu-id="2e3c3-113">Congratulations!</span></span> <span data-ttu-id="2e3c3-114">Теперь вы готовы к созданию интеллектуальных приложений с помощью инструментария Azure.</span><span class="sxs-lookup"><span data-stu-id="2e3c3-114">You're now ready to start building intelligent applications with Azure tooling.</span></span> <span data-ttu-id="2e3c3-115">Пример приложения и дополнительную документацию см. в статье о [подключении данных репозитория GitHub в Microsoft Graph](https://github.com/OfficeDev/MS-Graph-Data-Connect/wiki).</span><span class="sxs-lookup"><span data-stu-id="2e3c3-115">For a sample application and additional documentation, see the [Microsoft Graph data connect GitHub repo](https://github.com/OfficeDev/MS-Graph-Data-Connect/wiki).</span></span> 

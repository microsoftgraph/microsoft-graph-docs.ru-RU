---
title: Установка SDK Graph Microsoft Graph PowerShell
description: Содержит инструкции по установке SDK Graph PowerShell.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 58e967d7acedbbfe4f8c3781a7ec796e697a44c8
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53107678"
---
# <a name="install-the-microsoft-graph-powershell-sdk"></a><span data-ttu-id="d1978-103">Установка SDK Graph Microsoft Graph PowerShell</span><span class="sxs-lookup"><span data-stu-id="d1978-103">Install the Microsoft Graph PowerShell SDK</span></span>

> [!NOTE]
> <span data-ttu-id="d1978-104">Установка основного модуля SDK установит все 38 модулей.</span><span class="sxs-lookup"><span data-stu-id="d1978-104">Installing the main module of the SDK will install all 38 sub modules.</span></span> <span data-ttu-id="d1978-105">Рассмотрим только установку необходимых модулей, в том числе `Microsoft.Graph.Authentication` .</span><span class="sxs-lookup"><span data-stu-id="d1978-105">Consider only installing the neccessary modules, including `Microsoft.Graph.Authentication`.</span></span>

<span data-ttu-id="d1978-106">SDK Graph Microsoft Graph PowerShell опубликован в [галерее PowerShell.](https://www.powershellgallery.com/packages/Microsoft.Graph)</span><span class="sxs-lookup"><span data-stu-id="d1978-106">The Microsoft Graph PowerShell SDK is published on the [PowerShell Gallery](https://www.powershellgallery.com/packages/Microsoft.Graph).</span></span> <span data-ttu-id="d1978-107">Можно установить SDK в PowerShell Core или Windows PowerShell с помощью следующей команды.</span><span class="sxs-lookup"><span data-stu-id="d1978-107">You can install the SDK in PowerShell Core or Windows PowerShell using the following command.</span></span>

```powershell
Install-Module Microsoft.Graph -Scope CurrentUser
```

<span data-ttu-id="d1978-108">Необязательно можно изменить область установки с помощью `-Scope` параметра.</span><span class="sxs-lookup"><span data-stu-id="d1978-108">Optionally, you can change the scope of the installation using the `-Scope` parameter.</span></span> <span data-ttu-id="d1978-109">Для этого требуются разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="d1978-109">This requires admin permissions.</span></span>

```powershell
Install-Module Microsoft.Graph -Scope AllUsers
```

> [!IMPORTANT]
> <span data-ttu-id="d1978-110">Установка SDK в одной версии PowerShell не устанавливает его для другой.</span><span class="sxs-lookup"><span data-stu-id="d1978-110">Installing the SDK in one version of PowerShell does not install it for the other.</span></span> <span data-ttu-id="d1978-111">Не забудьте запустить команду установки в версии PowerShell, в которая вы собираетесь использовать ее.</span><span class="sxs-lookup"><span data-stu-id="d1978-111">Be sure to run the installation command inside the version of PowerShell you intend to use it in.</span></span>

## <a name="verify-installation"></a><span data-ttu-id="d1978-112">Проверка установки</span><span class="sxs-lookup"><span data-stu-id="d1978-112">Verify installation</span></span>

<span data-ttu-id="d1978-113">После завершения установки можно проверить установленную версию следующей командой.</span><span class="sxs-lookup"><span data-stu-id="d1978-113">After the installation completes, you can verify the installed version with the following command.</span></span>

```powershell
Get-InstalledModule Microsoft.Graph
```

<span data-ttu-id="d1978-114">Версия в выходе должна соответствовать последней версии, опубликованной в Галерее PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d1978-114">The version in the output should match the latest version published on the PowerShell Gallery.</span></span> <span data-ttu-id="d1978-115">Теперь вы готовы использовать SDK.</span><span class="sxs-lookup"><span data-stu-id="d1978-115">Now you're ready to use the SDK.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="d1978-116">Начало работы с SDK Microsoft Graph PowerShell</span><span class="sxs-lookup"><span data-stu-id="d1978-116">Get started with the Microsoft Graph PowerShell SDK</span></span>](get-started.md)

## <a name="updating-the-sdk"></a><span data-ttu-id="d1978-117">Обновление SDK</span><span class="sxs-lookup"><span data-stu-id="d1978-117">Updating the SDK</span></span>

<span data-ttu-id="d1978-118">Вы можете обновить SDK и все его зависимости с помощью следующей команды.</span><span class="sxs-lookup"><span data-stu-id="d1978-118">You can update the SDK and all of its dependencies using the following command.</span></span>

```powershell
Update-Module Microsoft.Graph
```

## <a name="uninstalling-the-sdk"></a><span data-ttu-id="d1978-119">Uninstalling the SDK</span><span class="sxs-lookup"><span data-stu-id="d1978-119">Uninstalling the SDK</span></span>

<span data-ttu-id="d1978-120">Сначала используйте следующую команду, чтобы удалить основной модуль.</span><span class="sxs-lookup"><span data-stu-id="d1978-120">First, use the following command to uninstall the main module.</span></span>

```powershell
Uninstall-Module Microsoft.Graph
```

<span data-ttu-id="d1978-121">Затем удалите все модули зависимостей, запуская следующие команды.</span><span class="sxs-lookup"><span data-stu-id="d1978-121">Then, remove all of the dependency modules by running the following commands.</span></span>

```powershell
Get-InstalledModule Microsoft.Graph.* | %{ if($_.Name -ne "Microsoft.Graph.Authentication"){ Uninstall-Module $_.Name } }
Uninstall-Module Microsoft.Graph.Authentication
```

## <a name="provide-feedback"></a><span data-ttu-id="d1978-122">Предоставление отзывов</span><span class="sxs-lookup"><span data-stu-id="d1978-122">Provide feedback</span></span>

<span data-ttu-id="d1978-123">Мы приветствуем отзывы!</span><span class="sxs-lookup"><span data-stu-id="d1978-123">We welcome feedback!</span></span> <span data-ttu-id="d1978-124">Просьба предоставить любые отзывы или сообщить о проблемах в репозитории [SDK GitHub.](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues)</span><span class="sxs-lookup"><span data-stu-id="d1978-124">Please provide any feedback or report any problems on the [SDK GitHub repository](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues).</span></span>

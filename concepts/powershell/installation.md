---
title: Установка пакета SDK PowerShell для Microsoft Graph
description: Содержит инструкции по установке пакета SDK PowerShell для Microsoft Graph.
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 245cf03c8edf04a43c563bd19832eb0a35cf7cff
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193713"
---
# <a name="install-the-microsoft-graph-powershell-sdk"></a><span data-ttu-id="b5226-103">Установка пакета SDK PowerShell для Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b5226-103">Install the Microsoft Graph PowerShell SDK</span></span>

<span data-ttu-id="b5226-104">Пакет SDK Microsoft Graph PowerShell опубликован в [коллекции PowerShell](https://www.powershellgallery.com/packages/Microsoft.Graph).</span><span class="sxs-lookup"><span data-stu-id="b5226-104">The Microsoft Graph PowerShell SDK is published on the [PowerShell Gallery](https://www.powershellgallery.com/packages/Microsoft.Graph).</span></span> <span data-ttu-id="b5226-105">Вы можете установить пакет SDK в PowerShell Core или Windows PowerShell с помощью следующей команды.</span><span class="sxs-lookup"><span data-stu-id="b5226-105">You can install the SDK in PowerShell Core or Windows PowerShell using the following command.</span></span>

```powershell
Install-Module Microsoft.Graph
```

<span data-ttu-id="b5226-106">При необходимости вы можете изменить область установки по умолчанию с помощью `-Scope` параметра.</span><span class="sxs-lookup"><span data-stu-id="b5226-106">Optionally, you can change the default scope of the installation using the `-Scope` parameter.</span></span> <span data-ttu-id="b5226-107">Для этого требуются разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="b5226-107">This requires admin permissions.</span></span>

```powershell
Install-Module Microsoft.Graph -Scope AllUsers
```

> [!IMPORTANT]
> <span data-ttu-id="b5226-108">Установка пакета SDK в одной версии PowerShell не устанавливает ее для другого.</span><span class="sxs-lookup"><span data-stu-id="b5226-108">Installing the SDK in one version of PowerShell does not install it for the other.</span></span> <span data-ttu-id="b5226-109">Не забудьте выполнить команду установки в той версии PowerShell, в которой вы планируете ее использовать.</span><span class="sxs-lookup"><span data-stu-id="b5226-109">Be sure to run the installation command inside the version of PowerShell you intend to use it in.</span></span>

## <a name="verify-installation"></a><span data-ttu-id="b5226-110">Проверка установки</span><span class="sxs-lookup"><span data-stu-id="b5226-110">Verify installation</span></span>

<span data-ttu-id="b5226-111">После завершения установки можно проверить установленную версию с помощью следующей команды.</span><span class="sxs-lookup"><span data-stu-id="b5226-111">After the installation completes, you can verify the installed version with the following command.</span></span>

```powershell
Get-InstalledModule Microsoft.Graph
```

<span data-ttu-id="b5226-112">Версия в выходных данных должна отличаться от последней версии, опубликованной в галерее PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b5226-112">The version in the output should match the latest version published on the PowerShell Gallery.</span></span> <span data-ttu-id="b5226-113">Теперь вы готовы использовать пакет SDK.</span><span class="sxs-lookup"><span data-stu-id="b5226-113">Now you're ready to use the SDK.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="b5226-114">Начало работы с пакетом SDK PowerShell для Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b5226-114">Get started with the Microsoft Graph PowerShell SDK</span></span>](get-started.md)

## <a name="updating-the-sdk"></a><span data-ttu-id="b5226-115">Обновление пакета SDK</span><span class="sxs-lookup"><span data-stu-id="b5226-115">Updating the SDK</span></span>

<span data-ttu-id="b5226-116">Вы можете обновить пакет SDK и все его зависимости с помощью следующей команды.</span><span class="sxs-lookup"><span data-stu-id="b5226-116">You can update the SDK and all of its dependencies using the following command.</span></span>

```powershell
Update-Module Microsoft.Graph
```

## <a name="uninstalling-the-sdk"></a><span data-ttu-id="b5226-117">Удаление пакета SDK</span><span class="sxs-lookup"><span data-stu-id="b5226-117">Uninstalling the SDK</span></span>

<span data-ttu-id="b5226-118">Сначала удалите основной модуль с помощью следующей команды.</span><span class="sxs-lookup"><span data-stu-id="b5226-118">First, use the following command to uninstall the main module.</span></span>

```powershell
Uninstall-Module Microsoft.Graph
```

<span data-ttu-id="b5226-119">Затем удалите все модули зависимости, выполнив указанные ниже команды.</span><span class="sxs-lookup"><span data-stu-id="b5226-119">Then, remove all of the dependency modules by running the following commands.</span></span>

```powershell
Get-InstalledModule Microsoft.Graph.* | %{ if($_.Name -ne "Microsoft.Graph.Authentication"){ Uninstall-Module $_.Name } }
Uninstall-Module Microsoft.Graph.Authentication
```

## <a name="provide-feedback"></a><span data-ttu-id="b5226-120">Предоставление отзывов</span><span class="sxs-lookup"><span data-stu-id="b5226-120">Provide feedback</span></span>

<span data-ttu-id="b5226-121">Мы ждем отзывов!</span><span class="sxs-lookup"><span data-stu-id="b5226-121">We welcome feedback!</span></span> <span data-ttu-id="b5226-122">Сообщите о любой обратной связи или сообщите о проблемах в [репозитории GitHub SDK](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues).</span><span class="sxs-lookup"><span data-stu-id="b5226-122">Please provide any feedback or report any problems on the [SDK GitHub repository](https://github.com/microsoftgraph/msgraph-sdk-powershell/issues).</span></span>

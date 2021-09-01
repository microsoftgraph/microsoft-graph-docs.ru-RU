---
title: тип enum policySetStatus
description: В этом переустановлении указывается состояние PolicySet.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 384eb054757e2a71ff15b4af45d91cc940416adb
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58757904"
---
# <a name="policysetstatus-enum-type"></a>тип enum policySetStatus

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

В этом переустановлении указывается состояние PolicySet.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|unknown|0|Значение по умолчанию.|
|проверка|1|Все элементы PolicySet теперь являются проверкой для соответствующих параметров рабочих нагрузок.|
|partialSuccess|2|После завершения процесса для всех элементов PolicySet, но есть сбои.|
|success|3|Развертываются все элементы PolicySet. Это не значит, что все развертывание успешно. |
|error|4 |Обработка PolicySet полностью провалилась.|
|notAssigned|5 |PolicySet/PolicySetItem не назначена ни одной группе.|




---
title: Политики и выставление счетов для подключения к данным Microsoft Graph
description: Описание поддерживаемых политик и модели выставления счетов Подключения к данным.
author: fercobo-msft
ms.localizationpriority: high
ms.prod: data-connect
ms.openlocfilehash: 83c285d94a060f5e66c76e27ab041a04c4da8d7a
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176587"
---
# <a name="microsoft-graph-data-connect-policies-and-billing"></a>Политики и выставление счетов для подключения к данным Microsoft Graph

Подключение к данным Microsoft Graph осуществляется с помощью [управляемых приложений Azure](/azure/managed-applications/overview). С их помощью вы можете создать и развернуть решения в среде Azure. С помощью управляемых приложений вы можете поддерживать определенные политики Azure, обеспечивая клиентам более высокий доверительный уровень и комфорт при использовании приложений.

## <a name="policies"></a>Политики

Управляемые приложения Azure, созданные на основе данных Microsoft 365, поддерживают следующие политики Azure:

- [Встроенные определения политики Azure для службы хранилища Azure](/azure/storage/common/policy-reference)
- [Введение в Azure Data Lake Storage 2-го поколения](/azure/storage/blobs/data-lake-storage-introduction)
- [Встроенные определения политики Azure для Azure Data Lake Storage 1-го поколения](/azure/data-lake-store/policy-reference)

> [!NOTE]
> Azure Data Lake Storage 1-го и 2-го поколения используют разные политики, поскольку Azure Data Lake Storage 2-го поколения реализует службу хранилища Azure.

После проверки состояния соответствия политике, выбранной во время публикации в Azure Marketplace, она применяется ко всем установленным экземплярам приложения. Все выбранные политики, которые соответствуют требованиям, отображаются для лиц, утверждающих данные, в рамках запроса данных. В случае нарушения соответствия политике происходит сбой в работе канала и прекращается извлечение данных.

## <a name="billing"></a>Выставление счетов

Счет связан с подпиской Azure Фабрики данных Azure, которую вы используете. Цена в этой новой модели выставления счетов зависит от количества объектов Microsoft Graph, к которым вы обращаетесь. Дополнительные сведения о выставлении счетов см. на странице [Цены](https://azure.microsoft.com/pricing/details/graph-data-connect/).

Объекты каталога, за которые не взимается плата:

- BasicDataSet_v0.User
- BasicDataSet_v0.MailboxSettings
- BasicDataSet_v0.Manager
- BasicDataSet_v0.DirectReport

## <a name="see-also"></a>См. также

- [Выбор и фильтрация пользователей](data-connect-filtering.md)
- [Вопросы и ответы о подключении к данным](data-connect-faq.md)

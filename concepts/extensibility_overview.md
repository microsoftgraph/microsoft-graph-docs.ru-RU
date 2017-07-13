<span data-ttu-id="bb5ad-p116">Для чтения или записи данных расширений в ресурсе необходимы те же [разрешения](./permissions_reference.md), что и для чтения или записи ресурса. Например, чтобы приложение могло добавить данные в профиль пользователя, который вошел в учетную запись, у него должно быть разрешение *User.ReadWrite.All*.</span><span class="sxs-lookup"><span data-stu-id="bb5ad-p116">The same [permissions](./permissions_reference.md) that are required to read from or write to a specific resource are also required to read from or write to any extensions data on that resource.  For example, for an app to be able to update the signed-in user's profile with custom app data, the app must have been granted the *User.ReadWrite.All* permission.</span></span>

Для чтения или записи данных расширений в ресурсе необходимы те же [разрешения](./permissions_reference.md), что и для чтения или записи ресурса. Например, чтобы приложение могло добавить данные в профиль пользователя, который вошел в учетную запись, у него должно быть разрешение *User.ReadWrite.All*.

<span data-ttu-id="bb5ad-229">Кроме того, для создания определений расширения схемы и управления ими приложению необходимо разрешение *Directory.AccessAsUser.All*.</span><span class="sxs-lookup"><span data-stu-id="bb5ad-229">Additionally, to create and manage schema extension definitions, an application must be granted the *Directory.AccessAsUser.All* permission.</span></span>

## <span data-ttu-id="bb5ad-230">Ограничения данных</span><span class="sxs-lookup"><span data-stu-id="bb5ad-230">Data limits</span></span>
<a id="data-limits" class="xliff"></a>

### <span data-ttu-id="bb5ad-231">Ограничения открытых расширений</span><span class="sxs-lookup"><span data-stu-id="bb5ad-231">Open extension limits</span></span>
<a id="open-extension-limits" class="xliff"></a>
<span data-ttu-id="bb5ad-232">К ресурсам каталогов, таким как **user**, **group**, **device**, применимы следующие ограничения:</span><span class="sxs-lookup"><span data-stu-id="bb5ad-232">The following limits apply to directory resources (such as **user**, **group**, **device**):</span></span>

- <span data-ttu-id="bb5ad-233">Каждое открытое расширение может содержать до 2 КБ данных (включая само определение расширения).</span><span class="sxs-lookup"><span data-stu-id="bb5ad-233">Each open extension can have up to 2KB of data (including the extension definition itself).</span></span>
- <span data-ttu-id="bb5ad-234">Приложение может создавать до двух открытых расширений для каждого экземпляра ресурса.</span><span class="sxs-lookup"><span data-stu-id="bb5ad-234">An application can add up to two open extensions per resource instance.</span></span>

### <span data-ttu-id="bb5ad-235">Ограничения расширений схемы</span><span class="sxs-lookup"><span data-stu-id="bb5ad-235">Schema extension limits</span></span>
<a id="schema-extension-limits" class="xliff"></a>
<span data-ttu-id="bb5ad-236">Приложение может создать не более пяти определений **расширений схемы**.</span><span class="sxs-lookup"><span data-stu-id="bb5ad-236">An application may create no more than five **schema extension** definitions.</span></span>

## <span data-ttu-id="bb5ad-237">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="bb5ad-237">Known limitations</span></span>
<a id="known-limitations" class="xliff"></a>

<span data-ttu-id="bb5ad-238">Об известных ограничениях на использование расширений можно узнать в [соответствующем разделе](known_issues.md#extensions) статьи об известных проблемах.</span><span class="sxs-lookup"><span data-stu-id="bb5ad-238">For known limitations using extensions, see the [extensions section](known_issues.md#extensions) in the known issues article.</span></span>

## <span data-ttu-id="bb5ad-239">Примеры расширений</span><span class="sxs-lookup"><span data-stu-id="bb5ad-239">Extension examples</span></span>
<a id="extension-examples" class="xliff"></a>

[<span data-ttu-id="bb5ad-240">Добавление пользовательских данных в ресурсы user с помощью открытых расширений</span><span class="sxs-lookup"><span data-stu-id="bb5ad-240">Add custom data to users using open extensions</span></span>](extensibility_open_users.md)

[<span data-ttu-id="bb5ad-241">Добавление пользовательских данных в группы с помощью расширений схемы</span><span class="sxs-lookup"><span data-stu-id="bb5ad-241">Add custom data to groups using schema extensions</span></span>](extensibility_schema_groups.md)

## <span data-ttu-id="bb5ad-242">См. также</span><span class="sxs-lookup"><span data-stu-id="bb5ad-242">See also</span></span>
<a id="see-also" class="xliff"></a>

<span data-ttu-id="bb5ad-243">
  [Домены Office 365](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)</span><span class="sxs-lookup"><span data-stu-id="bb5ad-243">[Office 365 domains](https://technet.microsoft.com/en-us/library/office-365-domains.aspx)</span></span>

[<span data-ttu-id="bb5ad-244">Добавление и подтверждение домена для клиента Office 365</span><span class="sxs-lookup"><span data-stu-id="bb5ad-244">Adding and verifying a domain for an Office 365 tenant</span></span>](http://office365support.ca/adding-and-verifying-a-domain-for-the-new-office-365/)
